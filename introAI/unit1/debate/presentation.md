<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Intro to AI Debate</title>
<style>
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  background: #111;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.slide {
  display: none;
  text-align: center;
  font-size: 4rem;
}

.active {
  display: block;
}

.hint {
  position: absolute;
  bottom: 20px;
  font-size: 14px;
  opacity: 0.6;
}
</style>
</head>
<body>

<div class="slide active">Intro to AI Debate</div>
<div class="slide">Introductions</div>
<div class="slide">Opening Statements</div>
<div class="slide">Rebuttals</div>
<div class="slide">Cross Examination</div>
<div class="slide">Closing Statements</div>
<div class="slide">Conclusion</div>

<div class="hint">Use ← → arrow keys or spacebar</div>

<script>
const slides = document.querySelectorAll('.slide');
let index = 0;

function showSlide(i) {
  slides[index].classList.remove('active');
  index = (i + slides.length) % slides.length;
  slides[index].classList.add('active');
}

document.addEventListener('keydown', (e) => {
  if (e.key === 'ArrowRight' || e.key === ' ') showSlide(index + 1);
  if (e.key === 'ArrowLeft') showSlide(index - 1);
});
</script>

</body>
</html>
