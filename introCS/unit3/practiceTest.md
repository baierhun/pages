# **Unit 3 Practice Test**

### **1.**

Which condition correctly checks if the mouse is in the **top half** of the canvas? **(1 point)**

* A. `mouseY < 200`
* B. `mouseY > 200`
* C. `mouseX < 200`
* D. `mouseX > 200`

---

### **2.**

Which event handler correctly runs when a key is pressed? **(1 point)**

* A. `onKey()`
* B. `onKeyPress(key)`
* C. `onPressKey()`
* D. `keyPress()`

---

### **3.**

What does this code check?

```python
if circle.hits(mouseX, mouseY):
```

* A. If the mouse is inside the circle
* B. If the circle touches another shape
* C. If two shapes overlap
* D. If the mouse is outside the canvas

---

### **4.**

What does this code check?

```python
if ball.hitsShape(rect):
```

* A. If the mouse touches the ball
* B. If the ball touches the rectangle
* C. If the rectangle is inside the ball
* D. If the ball is inside the mouse

---

<div class="break"></div>


### **5.**

What happens when the key `"space"` is pressed?

```python
def onKeyPress(key):
    if key == "space":
        ball.fill = "red"
```

* A. The ball turns red
* B. The ball turns red then back to black on release
* C. The program crashes
* D. Nothing happens

---

### **6.**

What shapes are drawn when the mouse is clicked at (250, 250)? **(1 point)**

```python
def onMousePress(mouseX, mouseY):
    if mouseX > 200:
        Circle(mouseX, mouseY, 80, fill='blue')
    if mouseY > 200:
        Circle(mouseX, mouseY, 40, fill='green')
    else:
        Circle(mouseX, mouseY, 40, fill='red')
```

* A. Blue and green circles
* B. Blue and red circles
* C. Only a blue circle
* D. Only a green circle

---

### **7.**

Which program correctly moves a ball to the right every step? **(1 point)**
<table class="answer-table">
<tr>
<td>
A.

```python
ball.centerX = ball.centerX - 5
```
</td><td>
B.

```python
ball.centerX += 5
```
</td></tr><tr><td>
C.

```python
ball.centerY += 5
```
</td><td>
D.

```python
ball.speed = ball.speed - 5
```
</tr></td></table>

---

### **8.**

What is wrong with this code? **(1 point)**

```python
def onStep()
    ball.centerY += 5
```

* A. Missing colon after event handler definition
* B. Missing parentheses in event handler name
* C. Missing `onMousePress`
* D. Nothing is wrong

---

### **9.**

When does this circle turn green?

```python
def onMousePress(mouseX, mouseY):
    if mouseX < 150:
        c.fill = "green"
```

* A. When mouseX is less than 150
* B. When mouseX is greater than 150
* C. Always
* D. Never

---

### **10.**

What happens after 2 steps?

```python
ball = Circle(100, 100, 20)
ball.dx = 10

def onStep():
    ball.centerX += ball.dx
```

* A. Ball moves right to 120
* B. Ball moves right to 110
* C. Ball moves left to 120
* D. Ball moves up to 110

---

<div class="break"></div>

### **11.**

What will happen after 4 mouse clicks at (100, 100)?

```python
def onMousePress(mouseX, mouseY):
    if mouseX < 200:
        c.fill = "red"
    else:
        c.fill = "blue"
```

* A. The circle alternates red and blue every click
* B. The circle is always red
* C. The circle is always blue
* D. The circle never changes color

---

### **12.**

Which statement is TRUE about this code?

```python
if rect.hits(ball.centerX, ball.centerY):
    rect.fill = "green"
```

* A. It checks if the rectangle touches the ball shape
* B. It checks if the ball's center is touching any part of rect
* C. It only works if both shapes are circles
* D. It checks if two shapes are identical

---

### **13.**

What happens when the spacebar is pressed 3 times?

```python
def onKeyPress(key):
    if key == "space":
        ball.centerY -= 10
```

* A. The ball moves up 10 total
* B. The ball moves up 30 total
* C. The ball moves down 30 total
* D. The ball does not move

---

<div class="break"></div>

### **14.**

Which condition correctly detects if **two shapes are touching each other**?

* A. `shape1.hits(shape2.centerX, shape2.centerY)`
* B. `shape1.hitsShape(shape2)`
* C. `shape1.hits(mouseX, mouseY)`
* D. `shape1.overlaps(mouseX, mouseY)`

---

### **15.**

What is the result after 3 steps?

```python
ball = Circle(200, 200, 20)
ball.dy = 5

def onStep():
    ball.centerY += ball.dy
    ball.dy += 1
```

* A. The ball moves the same distance each step
* B. The ball slows down over time
* C. The ball speeds up over time
* D. The ball does not move

---

<div class="break"></div>


# **Answer Key**

| Q# | Answer |
| -- | ------ |
| 1  | B      |
| 2  | B      |
| 3  | A      |
| 4  | B      |
| 5  | A      |
| 6  | A      |
| 7  | B      |
| 8  | A      |
| 9  | A      |
| 10 | A      |
| 11 | B      |
| 12 | B      |
| 13 | B      |
| 14 | B      |
| 15 | C      |
