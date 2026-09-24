<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Guess the Fruit</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 2rem;
      background-color: #f9f9f9;
    }
    img {
      width: 200px;
      height: 200px;
      border: 2px solid #333;
      margin-bottom: 1rem;
    }
    button {
      margin: 0.5rem;
      padding: 0.5rem 1rem;
      font-size: 1rem;
      cursor: pointer;
    }
    #fruitName {
      font-weight: bold;
      font-size: 1.2rem;
      margin-top: 1rem;
      display: none; /* Hidden until revealed */
    }
    #instructions {
      margin-bottom: 1rem;
      font-style: italic;
    }
    input {
      margin: 0.5rem;
      padding: 0.4rem;
      width: 200px;
      font-size: 1rem;
    }
  </style>
</head>
<body>

  <h1>Guess the Fruit!</h1>
  <p id="instructions">
    Look at this fruit image. Based on your definition instructions, is this your target fruit? Make a guess before revealing the answer!
  </p>
  
  <img id="fruitImage" src="" alt="Fruit Image">
  
  <div>
    <button id="nextFruitBtn">Show Random Fruit</button>
    <button id="revealBtn">Reveal Fruit</button>
  </div>

  <div>
    <input type="text" id="searchInput" placeholder="Enter fruit ID to search">
    <button id="searchBtn">Search</button>
  </div>
  
  <p id="fruitName"></p>

  <script>
    let fruits = [];
    let currentFruit = null;

    const fruitImage = document.getElementById('fruitImage');
    const fruitName = document.getElementById('fruitName');
    const nextBtn = document.getElementById('nextFruitBtn');
    const revealBtn = document.getElementById('revealBtn');
    const searchBtn = document.getElementById('searchBtn');
    const searchInput = document.getElementById('searchInput');

    // Load data.json
    fetch('data.json')
      .then(response => response.json())
      .then(data => {
        fruits = data;
        showRandomFruit(); // show first fruit
      })
      .catch(err => console.error('Error loading data.json:', err));

    function showRandomFruit() {
      if (fruits.length === 0) return;
      const randomIndex = Math.floor(Math.random() * fruits.length);
      currentFruit = fruits[randomIndex];

      fruitImage.src = currentFruit.url;
      fruitName.style.display = 'none';
      fruitName.textContent = currentFruit.id;
    }

    function revealFruit() {
      if (currentFruit) {
        fruitName.style.display = 'block';
      }
    }

    function searchFruit() {
      const searchTerm = searchInput.value.trim();
      if (!searchTerm) return;

      const found = fruits.find(f => f.id.toLowerCase() === searchTerm.toLowerCase());
      if (found) {
        currentFruit = found;
        fruitImage.src = found.url;
        fruitName.style.display = 'none';
        fruitName.textContent = found.id;
      } else {
        alert('Fruit not found. Check the ID.');
      }
    }

    nextBtn.addEventListener('click', showRandomFruit);
    revealBtn.addEventListener('click', revealFruit);
    searchBtn.addEventListener('click', searchFruit);

  </script>
</body>
</html>