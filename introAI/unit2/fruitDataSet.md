<html lang="en">
<head>
<meta charset="UTF-8">
<title>Random Fruit Selector 🍍🍎🍌</title>

<style>
  body {
    font-family: Arial, sans-serif;
    text-align: center;
    padding: 30px;
  }
  #fruit-img {
    margin-top: 20px;
    max-width: 400px;
    border: 2px solid #ddd;
    border-radius: 8px;
  }
  input, button {
    padding: 8px;
    margin: 6px;
    font-size: 16px;
  }
</style>
</head>
<body>

<h1>🍓 Random Fruit Image Viewer</h1>

<button onclick="randomFruit()">🎲 Pick Random Fruit</button>

<div style="margin-top: 20px;">
  <input type="text" id="search-box" placeholder="Enter unique ID" />
  <button onclick="searchById()">🔍 Search by ID</button>
</div>

<h3 id="fruit-id"></h3>
<img id="fruit-img" src="" alt="Fruit Image" />

<script>
// Global dataset
let fruits = [];

// Load the dataset
fetch('data.json')
  .then(resp => resp.json())
  .then(data => {
    fruits = data;
  })
  .catch(err => {
    console.error("Failed to load data.json:", err);
  });

// Pick a random fruit
function randomFruit() {
  if (fruits.length === 0) return;
  const idx = Math.floor(Math.random() * fruits.length);
  showFruit(fruits[idx]);
}

// Show fruit image & ID
function showFruit(item) {
  document.getElementById('fruit-id').textContent = "ID: " + item.id;
  document.getElementById('fruit-img').src = item.url;
  document.getElementById('fruit-img').alt = item.id;
}

// Search by unique ID
function searchById() {
  const id = document.getElementById('search-box').value.trim();
  if (!id) return alert("Enter a valid ID");

  const found = fruits.find(f => f.id === id);

  if (!found) {
    alert("No fruit found with that ID!");
    document.getElementById('fruit-img').src = "";
    document.getElementById('fruit-id').textContent = "";
    return;
  }

  showFruit(found);
}
</script>

</body>
</html>