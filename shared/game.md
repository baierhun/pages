<html lang="en">
<head>
<meta charset="UTF-8">
<title>Classroom Coding Games</title>

<style>
body {
    font-family: Arial;
    text-align: center;
    background: #f4f6f8;
    padding: 30px;
}

.controls {
    margin-bottom: 20px;
}

#question {
    font-size: 24px;
    margin: 20px auto;
    padding: 20px;
    background: white;
    border-radius: 10px;
    display: block;
    text-align: left;

    white-space: pre-wrap;
    word-wrap: break-word;
    overflow-wrap: break-word;

    max-width: 600px;
}

#answer {
    font-size: 22px;
    margin: 15px;
    color: green;
    visibility: hidden;
}

button {
    padding: 8px 12px;
    margin: 5px;
    border: none;
    border-radius: 6px;
    cursor: pointer;
}

.main-btn {
    background: #007bff;
    color: white;
}

.round-btn {
    background: #6c757d;
    color: white;
}

.scoreboard {
    margin-top: 30px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
}

.team {
    background: white;
    padding: 12px;
    border-radius: 10px;
    width: 140px;
}

.score {
    font-size: 26px;
    margin: 8px 0;
}

.team input {
    width: 100%;
    text-align: center;
}

/* Toggle container */
.toggle-container {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    margin-top: 10px;
    font-weight: bold;
    font-size: 14px; /* slightly smaller text */
}

/* Switch wrapper (smaller) */
.switch {
    position: relative;
    display: inline-block;
    width: 36px;   /* was 50px */
    height: 20px;  /* was 26px */
}

/* Hide default checkbox */
.switch input {
    opacity: 0;
    width: 0;
    height: 0;
}

/* Slider background */
.slider {
    position: absolute;
    cursor: pointer;
    inset: 0;
    background-color: #ccc;
    border-radius: 20px;
    transition: 0.25s;
}

/* Slider circle (scaled down) */
.slider:before {
    content: "";
    position: absolute;
    height: 14px;   /* was 20px */
    width: 14px;    /* was 20px */
    left: 3px;
    bottom: 3px;
    background-color: white;
    border-radius: 50%;
    transition: 0.25s;
}

/* Checked state */
.switch input:checked + .slider {
    background-color: #007bff;
}

.switch input:checked + .slider:before {
    transform: translateX(16px); /* adjusted for smaller width */
}

</style>
</head>

<body>

<h1>🎮 Classroom Coding Games</h1>

<div class="controls">
    <select id="gameSelect" onchange="loadSelectedGame()"></select>

    <div>
        <button class="round-btn" onclick="setRound(1)">🟢 Warm-Up</button>
        <button class="round-btn" onclick="setRound(2)">🟡 Challenge</button>
        <button class="round-btn" onclick="setRound(3)">🔴 Brain Burner</button>
    </div>
    <div class="toggle-container">
        <span>Ordered</span>

        <label class="switch">
            <input type="checkbox" id="randomToggle" checked>
            <span class="slider"></span>
        </label>

        <span>Random</span>
    </div>
</div>

<div>
    <span>Timer: </span>
    <span id="timerDisplay">00:00</span>
    <select id="timerMode">
        <option value="up">Count Up ⏱️</option>
        <option value="down">Count Down ⏲️</option>
    </select>
    <input type="number" id="timerStart" value="60" min="1" style="width: 60px;"> seconds
    <button class="main-btn" onclick="resetTimer()">Reset Timer</button>
</div>

<div id="question"></div>
<div id="answer"></div>

<button class="main-btn" onclick="showAnswer()">Show Answer</button>
<button class="main-btn" onclick="nextQuestion()">Next Question</button>
<button class="main-btn" id="prevBtn" onclick="prevQuestion()">Previous Question</button>

<div class="scoreboard" id="scoreboard"></div>

<button class="main-btn" onclick="addTeam()">➕ Add Team</button>
<button class="main-btn" onclick="removeTeam()">➖ Remove Team</button>

<script>
// ---------------- HELPERS ----------------
const rand = arr => arr[Math.floor(Math.random()*arr.length)];

// ---------------- GAME FILES ----------------
const gameFiles = [
    "games/data-types.md",
    "games/boolean-logic.md",
    "games/loop-practice.md"
];

let games = {};
let currentGameQuestions = [];

// ---------------- ROUND SYSTEM ----------------
let currentRound = 1;

function setRound(r) {
    currentRound = r;
    resetGameState();
    nextQuestion();
}

// ---------------- HISTORY ----------------
let history = [];
let historyIndex = -1;

// ---------------- NO REPEAT TRACKING ----------------
let unusedQuestions = [];

// ---------------- LOAD GAMES ----------------
async function loadGames() {
    for (let file of gameFiles) {
        let res = await fetch(file);
        let text = await res.text();
        let parsed = parseMarkdown(text);
        games[parsed.name] = parsed.questions;
    }
    populateDropdown();
}

// ---------------- PARSER ----------------
function parseMarkdown(md) {
    let nameMatch = md.match(/# Game Name:\s*(.*)/);
    let name = nameMatch ? nameMatch[1].trim() : "Game";

    let questions = [];
    let blocks = md.split("Q:");
    blocks.shift();

    for (let block of blocks) {
        let qMatch = block.match(/```([\s\S]*?)```/);
        let aMatch = block.match(/A:\s*(.*)/);
        let lMatch = block.match(/Level:\s*(.*)/);

        if (!qMatch || !aMatch || !lMatch) continue;

        questions.push({
            q: qMatch[1].trim(),
            a: aMatch[1].trim(),
            level: lMatch[1].trim()
        });
    }

    return { name, questions };
}

// ---------------- DROPDOWN ----------------
function populateDropdown() {
    let select = document.getElementById("gameSelect");

    for (let name in games) {
        let option = document.createElement("option");
        option.value = name;
        option.textContent = name;
        select.appendChild(option);
    }

    loadSelectedGame();
}

function loadSelectedGame() {
    let name = document.getElementById("gameSelect").value;
    currentGameQuestions = games[name];
    resetGameState();
    nextQuestion();
}

// ---------------- RESET STATE ----------------
function resetGameState() {
    history = [];
    historyIndex = -1;
    unusedQuestions = [];
}

// ---------------- FILTER BY LEVEL ----------------
function getQuestionPool() {
    let levelMap = {
        1: "warmup",
        2: "challenge",
        3: "brain"
    };

    return currentGameQuestions.filter(q => q.level === levelMap[currentRound]);
}

// ---------------- GAME ----------------
let timerInterval = null;
let timerSeconds = 0;
let timerCountingUp = true;

function startTimer() {
    clearInterval(timerInterval);

    const mode = document.getElementById("timerMode").value;
    const startValue = parseInt(document.getElementById("timerStart").value, 10);

    timerCountingUp = (mode === "up");
    timerSeconds = timerCountingUp ? 0 : startValue;

    updateTimerDisplay();

    timerInterval = setInterval(() => {
        if (timerCountingUp) {
            timerSeconds++;
        } else {
            timerSeconds--;
            if (timerSeconds <= 0) {
                clearInterval(timerInterval);
            }
        }
        updateTimerDisplay();
    }, 1000);
}

function updateTimerDisplay() {
    let minutes = Math.floor(timerSeconds / 60);
    let seconds = timerSeconds % 60;
    document.getElementById("timerDisplay").textContent =
        `${minutes.toString().padStart(2,'0')}:${seconds.toString().padStart(2,'0')}`;
}

function resetTimer() {
    clearInterval(timerInterval);
    const mode = document.getElementById("timerMode").value;
    const startValue = parseInt(document.getElementById("timerStart").value, 10);
    timerSeconds = timerCountingUp ? 0 : startValue;
    updateTimerDisplay();
}

function nextQuestion() {
    startTimer();

    let pool = getQuestionPool();
    if (pool.length === 0) return;

    // refill if empty
    if (unusedQuestions.length === 0) {
        unusedQuestions = [...pool];
    }

    const isRandom = document.getElementById("randomToggle").checked;

    let q;

    if (isRandom) {
        // RANDOM MODE
        let index = Math.floor(Math.random() * unusedQuestions.length);
        q = unusedQuestions.splice(index, 1)[0];
    } else {
        // ORDERED MODE
        q = unusedQuestions.shift();
    }

    history = history.slice(0, historyIndex + 1);
    history.push(q);
    historyIndex = history.length - 1;

    displayQuestion(q);
    updatePrevButton();
}

function prevQuestion() {
    if (history.length === 0) return;

    if (historyIndex > 0) {
        historyIndex--;
    }

    let q = history[historyIndex];
    if (q) displayQuestion(q);

    updatePrevButton();
}

function displayQuestion(q) {
    if (!q) return;

    document.getElementById("question").textContent = q.q;
    document.getElementById("answer").style.visibility = "hidden";
    document.getElementById("answer").textContent =
        "Answer: " + (q.a === "error" ? "Error ❌" : q.a);
}

function showAnswer() {
    document.getElementById("answer").style.visibility = "visible";
}

// ---------------- BUTTON STATE ----------------
function updatePrevButton() {
    document.getElementById("prevBtn").disabled = (historyIndex <= 0);
}

// ---------------- TEAMS ----------------
let teamCount = 0;

function addTeam() {
    teamCount++;

    let div = document.createElement("div");
    div.className = "team";
    div.id = "team"+teamCount;

    div.innerHTML = `
        <input value="Team ${teamCount}">
        <div id="score${teamCount}" class="score">0</div>
        <button onclick="changeScore(${teamCount},1)">+</button>
        <button onclick="changeScore(${teamCount},-1)">-</button>
    `;

    document.getElementById("scoreboard").appendChild(div);
}

function removeTeam() {
    if (teamCount <= 0) return;

    let el = document.getElementById("team"+teamCount);
    if (el) el.remove();

    teamCount--;
}

function changeScore(team, amt) {
    let el = document.getElementById("score"+team);
    el.textContent = parseInt(el.textContent)+amt;
}

// ---------------- INIT ----------------
addTeam();
addTeam();
loadGames();

document.getElementById("randomToggle")
    .addEventListener("change", () => {
        resetGameState();
        nextQuestion();
    });
</script>

</body>
</html>