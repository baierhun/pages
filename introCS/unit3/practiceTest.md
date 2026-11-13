<div class="title">
  <h1>Intro to CS — Unit 3 Practice Test</h1>
</div>

## Part I — Free Response

For Questions 1–4, assume these shapes already exist:

```python
ball = Circle(200, 200, 20, fill='blue')
target = Rect(300, 150, 50, 100, fill='gold')
```

##### 1. Mouse Position

Write an `onMousePress` event handler that changes the ball’s fill to green if the click is above the middle of the canvas. Otherwise, change its fill to purple.

<div style="height: 2in;"></div>

##### 2. Key Events

Write an `onKeyPress` event handler that:

- Moves the ball 10 to right when the right arrow is pressed.
- Moves the ball 10 to left when the left arrow is pressed.
- Does nothing when any other key is pressed.

<div class="break"></div>

##### 3. Clicking a Shape

Write an `onMousePress` event handler that increases the ball’s radius by 5 only if the click hits the ball.

<div style="height: 1.5in;"></div>

##### 4. Checking for Contact

Write an `onKeyPress` event handler that does the following when the right arrow is pressed:

1. Moves the ball 10 to right.
2. Checks whether the ball touches the target.
3. Changes the target’s fill to red if they touch, or gold otherwise.

<div style="height: 2in;"></div>

##### 5. Fix the Syntax

Rewrite the following code so it runs correctly.

```python
def onKeyPress(key):
    if key = 'up'
        ball.centerY -= 10
    else
        ball.centerY += 10
```

<div class="break"></div>

##### 6. Fix the Indentation

The programmer wants the ball to turn red only when the user clicks in the left half of the canvas. Rewrite the code correctly.

```python
def onMousePress(mouseX, mouseY):
    if mouseX < 200:
    ball.fill = 'red'
```

<div style="height: 1.25in;"></div>

##### 7. Fix the Logic

The programmer wants exactly one circle drawn per click:

- A red circle if the click is left of `x = 200`.
- A blue circle otherwise.

Explain the problem and rewrite the code.

```python
def onMousePress(mouseX, mouseY):
    if mouseX < 200:
        Circle(mouseX, mouseY, 20, fill='red')
    Circle(mouseX, mouseY, 20, fill='blue')
```

<div style="height: 1.75in;"></div>

##### 8. Fix the Method

The programmer wants to check whether two shapes touch. Rewrite the code using the correct method.

```python
if ball.hits(target):
    ball.fill = 'green'
```

<div class="break"></div>

## Part II — Multiple Choice

**Directions:** Select the best answer for each question.

##### 9. Which condition evaluates to `True`?

```python
traingle = Star(100, 200, 30, 3)
triangle.speedX = 200
triangle.speedY = 75
```

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> <span class="answer-code">triangle.speedX &lt; 200</span></td>
    <td><strong>B.</strong> <span class="answer-code">triangle.speedY != 75</span></td>
  </tr>
  <tr>
    <td><strong>C.</strong> <span class="answer-code">triangle.speedX &lt;= 200</span></td>
    <td><strong>D.</strong> <span class="answer-code">triangle.speedY &gt;= 100</span></td>
  </tr>
</table>

##### 10. What is the difference between `=` and `==`?

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> <span class="answer-code">=</span> assigns a value; <span class="answer-code">==</span> checks whether two values are equal.</td>
    <td><strong>B.</strong> <span class="answer-code">=</span> compares values; <span class="answer-code">==</span> assigns a value.</td>
  </tr>
  <tr>
    <td><strong>C.</strong> Both assign values.</td>
    <td><strong>D.</strong> Both compare values.</td>
  </tr>
</table>

##### 11. When does the indented code inside an `if` statement run?

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> Every time the program starts.</td>
    <td><strong>B.</strong> Only when the condition is <span class="answer-code">False</span>.</td>
  </tr>
  <tr>
    <td><strong>C.</strong> Only when the user presses a key.</td>
    <td><strong>D.</strong> When execution reaches the statement and its condition is <span class="answer-code">True</span>.</td>
  </tr>
</table>

##### 12. What does `ball.hits(mouseX, mouseY)` check?

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> Whether the ball touches another shape.</td>
    <td><strong>B.</strong> Whether the ball makes contact with the point <span class="answer-code">(mouseX, mouseY)</span>.</td>
  </tr>
  <tr>
    <td><strong>C.</strong> Whether the ball is moving.</td>
    <td><strong>D.</strong> Whether the mouse is on the left half of the canvas.</td>
  </tr>
</table>

<div class="break"></div>

##### 13. What shapes are drawn when the user clicks at `(100, 100)`?

```python
def onMousePress(mouseX, mouseY):
    if mouseX < 200:
        Circle(mouseX, mouseY, 20, fill='cyan')
    if mouseY < 200:
        Star(mouseX, mouseY, 30, 5, fill='gold')
```

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> Only a cyan circle.</td>
    <td><strong>B.</strong> Only a gold star.</td>
  </tr>
  <tr>
    <td><strong>C.</strong> A cyan circle and a gold star.</td>
    <td><strong>D.</strong> No shapes.</td>
  </tr>
</table>

##### 14. What color is the ball after the user clicks at `(200, 200)`?

```python
ball = Circle(200, 200, 20, fill='gray')

def onMousePress(mouseX, mouseY):
    if mouseX < 200:
        ball.fill = 'red'
    else:
        ball.fill = 'blue'
```

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> Red.</td>
    <td><strong>B.</strong> Blue.</td>
  </tr>
  <tr>
    <td><strong>C.</strong> Gray.</td>
    <td><strong>D.</strong> The code produces an error.</td>
  </tr>
</table>

##### 15. What is the ball’s final `centerX` after the user presses right, right, left, and space, in that order?

```python
ball = Circle(100, 200, 20)

def onKeyPress(key):
    if key == 'right':
        ball.centerX += 15
    if key == 'left':
        ball.centerX -= 10
```

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> <span class="answer-code">120</span></td>
    <td><strong>B.</strong> <span class="answer-code">130</span></td>
  </tr>
  <tr>
    <td><strong>C.</strong> <span class="answer-code">110</span></td>
    <td><strong>D.</strong> <span class="answer-code">100</span></td>
  </tr>
</table>

##### 16. Before running each version, the ball has a radius of `25` and a fill of `'blue'`. Which statement describes the final results?

**Version A**

```python
if ball.radius < 30:
    ball.radius += 10
if ball.radius >= 30:
    ball.fill = 'red'
```

**Version B**

```python
if ball.radius < 30:
    ball.radius += 10
else:
    ball.fill = 'red'
```

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> Both versions end with a radius of 35 and a red fill.</td>
    <td><strong>B.</strong> Both versions end with a radius of 35 and a blue fill.</td>
  </tr>
  <tr>
    <td><strong>C.</strong> Both end with a radius of 35. Version A is blue; Version B is red.</td>
    <td><strong>D.</strong> Both end with a radius of 35. Version A is red; Version B is blue.</td>
  </tr>
</table>

##### 17. The user clicks at `(125, 125)` and then at `(300, 300)`. What is the button’s fill after the second click?

```python
button = Rect(100, 100, 100, 50, fill='gray')

def onMousePress(mouseX, mouseY):
    if button.hits(mouseX, mouseY):
        button.fill = 'green'
    else:
        button.fill = 'gray'
```

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> Green.</td>
    <td><strong>B.</strong> Gray.</td>
  </tr>
  <tr>
    <td><strong>C.</strong> Blue.</td>
    <td><strong>D.</strong> The button disappears.</td>
  </tr>
</table>

<div class="break"></div>

##### 18. What happens when the user presses the up arrow?

```python
def onKeyPress(key):
    if key == 'space':
        ball.radius += 5
    else:
        ball.radius -= 2
```

<table class="mcq-choices">
  <tr>
    <td><strong>A.</strong> The ball’s radius increases by 5.</td>
    <td><strong>B.</strong> The ball moves up 2.</td>
  </tr>
  <tr>
    <td><strong>C.</strong> The ball’s radius decreases by 2.</td>
    <td><strong>D.</strong> Nothing happens.</td>
  </tr>
</table>

---

## Answer Key

##### 1. Mouse Position

```python
def onMousePress(mouseX, mouseY):
    if mouseY < 200:
        ball.fill = 'green'
    else:
        ball.fill = 'purple'
```

##### 2. Key Events

```python
def onKeyPress(key):
    if key == 'right':
        ball.centerX += 10
    if key == 'left':
        ball.centerX -= 10
```

##### 3. Clicking a Shape

```python
def onMousePress(mouseX, mouseY):
    if ball.hits(mouseX, mouseY):
        ball.radius += 5
```

<div class="break"></div>

##### 4. Checking for Contact

```python
def onKeyPress(key):
    if key == 'right':
        ball.centerX += 10
        if ball.hitsShape(target):
            target.fill = 'red'
        else:
            target.fill = 'gold'
```

##### 5. Fix the Syntax

```python
def onKeyPress(key):
    if key == 'up':
        ball.centerY -= 10
    else:
        ball.centerY += 10
```

##### 6. Fix the Indentation

```python
def onMousePress(mouseX, mouseY):
    if mouseX < 200:
        ball.fill = 'red'
```

##### 7. Fix the Logic

The blue circle is drawn on every click because its line is outside the `if` statement. Clicking on the left draws both circles.

```python
def onMousePress(mouseX, mouseY):
    if mouseX < 200:
        Circle(mouseX, mouseY, 20, fill='red')
    else:
        Circle(mouseX, mouseY, 20, fill='blue')
```

##### 8. Fix the Method

```python
if ball.hitsShape(target):
    ball.fill = 'green'
```

<div class="break"></div>

### Multiple-Choice Answers

| Question | Answer | Explanation |
|---|---|---|
| 9 | C | `200 <= 200` is `True`. |
| 10 | A | `=` assigns; `==` compares. |
| 11 | D | The condition must be `True` when the statement is reached. |
| 12 | B | `hits` checks contact with a point. |
| 13 | C | Both independent conditions are true. |
| 14 | B | `200 < 200` is false, so the `else` runs. |
| 15 | A | `100 + 15 + 15 - 10 = 120`. Space has no effect. |
| 16 | D | Version A checks its second condition after the radius changes. Version B skips the `else`. |
| 17 | B | The second click misses the button, so the `else` runs. |
| 18 | C | The up arrow is not space, so the `else` runs. |