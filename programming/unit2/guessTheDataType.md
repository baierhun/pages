<html lang="en">
<head>
<meta charset="UTF-8">
<title>Guess the Data Type!</title>
<style>
    body {
        font-family: Arial;
        text-align: center;
        background: #f4f6f8;
        padding: 30px;
    }

    #question {
        font-size: 24px;
        margin: 30px 0;
        padding: 20px;
        background: white;
        border-radius: 10px;
        display: inline-block;
        text-align: left;
        white-space: pre-line;
        min-width: 350px;
    }

    #answer {
        font-size: 24px;
        margin: 20px;
        color: green;
        visibility: hidden;
    }

    button {
        padding: 8px 12px;
        margin: 5px;
        border: none;
        border-radius: 6px;
        cursor: pointer;
        font-size: 14px;
    }

    .main-btn {
        background: #007bff;
        color: white;
    }

    .round-btn {
        background: #6c757d;
        color: white;
        font-size: 12px;
        padding: 6px 10px;
    }

    #roundDisplay {
        font-size: 20px;
        margin-top: 10px;
        font-weight: bold;
    }

    .scoreboard {
        margin-top: 40px;
        display: flex;
        justify-content: center;
        gap: 50px;
    }

    .team {
        background: white;
        padding: 20px;
        border-radius: 10px;
    }

    .team input {
        text-align: center;
        font-size: 18px;
    }

    .score {
        font-size: 32px;
        margin: 10px 0;
    }
</style>
</head>
<body>

<h1>🎯 Guess the Data Type!</h1>
<div id="roundDisplay">Round 1</div>

<div id="question"></div>
<div id="answer"></div>

<button class="main-btn" onclick="showAnswer()">Show Answer</button>
<button class="main-btn" onclick="nextQuestion()">Next Question</button>
<br>
<button class="round-btn" onclick="prevRound()">⬅️ Prev Round</button>
<button class="round-btn" onclick="nextRound()">Next Round ➡️</button>

<div class="scoreboard">
    <div class="team">
        <input value="Team 1">
        <div id="score1" class="score">0</div>
        <button onclick="changeScore(1,1)">+</button>
        <button onclick="changeScore(1,-1)">-</button>
    </div>

    <div class="team">
        <input value="Team 2">
        <div id="score2" class="score">0</div>
        <button onclick="changeScore(2,1)">+</button>
        <button onclick="changeScore(2,-1)">-</button>
    </div>
</div>

<script>
const intRange = () => Math.floor(Math.random()*10)+1;
const rand = arr => arr[Math.floor(Math.random()*arr.length)];
let round = 1;

// ---------- ROUND 1 ----------
function round1() {
    let a = intRange(), b = intRange(), c = intRange();
    let type = rand(["int","float","string","boolean","error"]);

    let options = {
        int: [
            `${a} + ${b}`,
            `${a} * ${b}`,
            `${a} // ${b}`,
            `${a} % ${b}`,
            `${a} + ${b} * ${c}`
        ],
        float: [
            `${a} / ${b}`,
            `${a}.0 + ${b}`,
            `${a} + ${b}.0`,
            `${a} / ${b} + ${c}`
        ],
        string: [
            `"hi"`,
            `"a" * ${a}`,
            `"hello" + "world"`
        ],
        boolean: [
            `${a} > ${b}`,
            `${a} == ${b}`,
            `${a} + ${b} > ${c}`
        ],
        error: [
            `"hi" + ${a}`,
            `${a} + "hi"`,
            `"a" - "b"`,
            `"x" / 2`
        ]
    };

    let chosen = rand(options[type]);
    return { q:`x = ${chosen}`, a:type };
}

// ---------- ROUND 2 ----------
function round2() {
    let a = intRange(), b = intRange();

    let lines = [
        `a = ${a}`,
        `b = ${b}`
    ];

    let type = rand(["int","float","string","boolean","error"]);

    if (type==="int") {
        lines.push(`c = a + b * 2`);
        lines.push(`d = c - a`);
    }
    else if (type==="float") {
        lines.push(`c = a / b`);
        lines.push(`d = c + 2`);
    }
    else if (type==="string") {
        lines.push(`c = "hi"`);
        lines.push(`d = c * a`);
    }
    else if (type==="boolean") {
        lines.push(`c = a + b`);
        lines.push(`d = c >= 5`);
    }
    else {
        lines.push(`c = "hi"`);
        lines.push(`d = c + a`);
    }

    return { q:lines.join("\n"), a:type };
}

// ---------- ROUND 3 ----------
function round3() {
    let a = intRange(), b = intRange();

    let lines = [
        `a = ${a}`,
        `b = ${b}`,
        `x = 999`, // distractor
        `a = a + 1`,
        `c = a * b + 3`
    ];

    let type = rand(["int","float","boolean","error"]);

    if (type==="int") {
        lines.push(`d = c // 2`);
    }
    else if (type==="float") {
        lines.push(`d = c / 2`);
    }
    else if (type==="boolean") {
        lines.push(`d = c > a * b`);
    }
    else {
        lines[4] = `c = "oops"`;
        lines.push(`d = c + a`);
    }

    return { q:lines.join("\n"), a:type };
}

// ---------- ROUND 4 ----------
function round4() {
    let data = round3();

    // extra randomness
    if (Math.random() < 0.5) {
        data.q = data.q.replace(`a = a + 1`, `a = a * 2`);
    }

    return data;
}

// ---------- GAME CONTROL ----------
function generateQuestion() {
    if (round===1) return round1();
    if (round===2) return round2();
    if (round===3) return round3();
    if (round===4) return round4();
}

function nextQuestion() {
    let q = generateQuestion();
    document.getElementById("question").textContent = q.q;
    document.getElementById("answer").style.visibility = "hidden";
    document.getElementById("answer").textContent =
        "Answer: " + (q.a==="error" ? "Error ❌" : q.a);
}

function showAnswer() {
    document.getElementById("answer").style.visibility = "visible";
}

function nextRound() {
    round++;
    if (round > 4) round = 1;
    updateRound();
}

function prevRound() {
    round--;
    if (round < 1) round = 4;
    updateRound();
}

function updateRound() {
    document.getElementById("roundDisplay").textContent = "Round " + round;
    nextQuestion();
}

function changeScore(team, amt) {
    let el = document.getElementById("score"+team);
    el.textContent = parseInt(el.textContent)+amt;
}

// start
nextQuestion();
</script>

</body>
</html>