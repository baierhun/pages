<div class="title">
    <h1>Unit 2 Practice Test</h1>
    <div class="print-on"><strong>Name:</strong>&nbsp;<span>&nbsp;</span></div>
</div>

---

### 1.

Which line correctly defines the code that should run when the mouse is pressed?

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong><span class="answer-code">def onMousePress(mouseX, mouseY)</span></td>
        <td><strong>B. </strong><span class="answer-code">def onMousePress(mouseX, mouseY):</span></td>
    </tr>
    <tr>
        <td><strong>C. </strong><span class="answer-code">def onMouseClick(mouseX, mouseY):</span></td>
        <td><strong>D. </strong><span class="answer-code">onMousePress(mouseX, mouseY):</span></td>
    </tr>
</table>

---

### 2.

What does `mouseX` represent inside `onMousePress(mouseX, mouseY)`?

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>The width of the canvas</td>
        <td><strong>B. </strong>The horizontal position of the mouse</td>
    </tr>
    <tr>
        <td><strong>C. </strong>The vertical position of the mouse</td>
        <td><strong>D. </strong>The radius of the shape being drawn</td>
    </tr>
</table>

---

### 3.

What will happen when the mouse is pressed at position (100, 150)?

<pre class="answer-code-block">def onMousePress(mouseX, mouseY):
    Circle(mouseX, mouseY, 25)</pre>

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>A circle appears at (25, 25).</td>
        <td><strong>B. </strong>A circle appears at (150, 100).</td>
    </tr>
    <tr>
        <td><strong>C. </strong>A circle appears at (100, 150).</td>
        <td><strong>D. </strong>A circle appears at (200, 200).</td>
    </tr>
</table>

---

### 4.

Which event should be used to make a shape respond continuously as the mouse moves?

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong><span class="answer-code">onMouseMove(mouseX, mouseY)</span></td>
        <td><strong>B. </strong><span class="answer-code">onMousePress(mouseX, mouseY)</span></td>
    </tr>
    <tr>
        <td><strong>C. </strong><span class="answer-code">onStep()</span></td>
        <td><strong>D. </strong><span class="answer-code">app.background</span></td>
    </tr>
</table>

<div class="break"></div>

### 5.

What is the value of `spot.centerX` after this code runs?

<pre class="answer-code-block">spot = Circle(100, 100, 20)
spot.centerX = 250</pre>

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>100</td>
        <td><strong>B. </strong>20</td>
    </tr>
    <tr>
        <td><strong>C. </strong>350</td>
        <td><strong>D. </strong>250</td>
    </tr>
</table>

---

### 6.

What is the height of `r` after this code runs?

<pre class="answer-code-block">r = Rect(10, 20, 40, 80)
r.height += 30</pre>

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>30</td>
        <td><strong>B. </strong>110</td>
    </tr>
    <tr>
        <td><strong>C. </strong>80</td>
        <td><strong>D. </strong>120</td>
    </tr>
</table>

---

### 7.

Which line moves a circle named `ball` 25 upward?

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong><span class="answer-code">ball.centerX -= 25</span></td>
        <td><strong>B. </strong><span class="answer-code">ball.centerY += 25</span></td>
    </tr>
    <tr>
        <td><strong>C. </strong><span class="answer-code">ball.centerY -= 25</span></td>
        <td><strong>D. </strong><span class="answer-code">ball.top = 25</span></td>
    </tr>
</table>

---

### 8.

What does the following code do?

<pre class="answer-code-block">box = Rect(50, 50, 100, 100)
box.width = box.width + 20</pre>

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>Changes the height to 120.</td>
        <td><strong>B. </strong>Moves the rectangle 20 right.</td>
    </tr>
    <tr>
        <td><strong>C. </strong>Sets the width to 20.</td>
        <td><strong>D. </strong>Increases the width to 120.</td>
    </tr>
</table>

<div class="break"></div>

### 9.

Which of the following is a size property of a shape?

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong><span class="answer-code">centerY</span></td>
        <td><strong>B. </strong><span class="answer-code">width</span></td>
    </tr>
    <tr>
        <td><strong>C. </strong><span class="answer-code">fill</span></td>
        <td><strong>D. </strong><span class="answer-code">rotateAngle</span></td>
    </tr>
</table>

---

### 10.

What does the following code do?

<pre class="answer-code-block">c = Circle(200, 200, 30)
c.fill = 'purple'</pre>

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>Changes the circle's radius to purple.</td>
        <td><strong>B. </strong>Moves the circle to the top-left corner.</td>
    </tr>
    <tr>
        <td><strong>C. </strong>Changes the circle's fill color to purple.</td>
        <td><strong>D. </strong>Changes the background color to purple.</td>
    </tr>
</table>

---

### 11.

What is the purpose of a custom property such as `ball.speedY`?

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>It stores additional information associated with the shape.</td>
        <td><strong>B. </strong>It automatically changes the shape's position.</td>
    </tr>
    <tr>
        <td><strong>C. </strong>It creates a second circle.</td>
        <td><strong>D. </strong>It changes the canvas background.</td>
    </tr>
</table>

---

### 12.

How many times per second does `onStep()` run by default?

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>1</td>
        <td><strong>B. </strong>10</td>
    </tr>
    <tr>
        <td><strong>C. </strong>60</td>
        <td><strong>D. </strong>30</td>
    </tr>
</table>

<div class="break"></div>

### 13.

What will be the value of `ball.centerY` after three steps?

<pre class="answer-code-block">ball = Circle(100, 100, 10)

def onStep():
    ball.centerY += 5</pre>

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>105</td>
        <td><strong>B. </strong>115</td>
    </tr>
    <tr>
        <td><strong>C. </strong>110</td>
        <td><strong>D. </strong>120</td>
    </tr>
</table>

---

### 14.

What is the value of `ball.centerY` after two steps?

<pre class="answer-code-block">ball = Circle(200, 200, 20)
ball.speedY = 10

def onStep():
    ball.centerY -= ball.speedY
    ball.speedY += 5</pre>

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong>175</td>
        <td><strong>B. </strong>180</td>
    </tr>
    <tr>
        <td><strong>C. </strong>170</td>
        <td><strong>D. </strong>185</td>
    </tr>
</table>

---

### 15.

Which line changes the canvas background to yellow?

<table class="mcq-choices">
    <tr>
        <td><strong>A. </strong><span class="answer-code">background = 'yellow'</span></td>
        <td><strong>B. </strong><span class="answer-code">app.fill = 'yellow'</span></td>
    </tr>
    <tr>
        <td><strong>C. </strong><span class="answer-code">app.background = 'yellow'</span></td>
        <td><strong>D. </strong><span class="answer-code">app.color = 'yellow'</span></td>
    </tr>
</table>

<br><br>

<div>
    <h3>Answer Key</h3>
    <table class="answer-key">
        <tr>
            <th>1</th>
            <th>2</th>
            <th>3</th>
            <th>4</th>
            <th>5</th>
            <th>6</th>
            <th>7</th>
            <th>8</th>
            <th>9</th>
            <th>10</th>
            <th>11</th>
            <th>12</th>
            <th>13</th>
            <th>14</th>
            <th>15</th>
        </tr>
        <tr>
            <td>B</td>
            <td>B</td>
            <td>C</td>
            <td>A</td>
            <td>D</td>
            <td>B</td>
            <td>C</td>
            <td>D</td>
            <td>B</td>
            <td>C</td>
            <td>A</td>
            <td>D</td>
            <td>B</td>
            <td>A</td>
            <td>C</td>
        </tr>
    </table>
</div>