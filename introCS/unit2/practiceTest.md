# **Unit 2 Practice Test**

### **1.**

Which of the following correctly defines a mouse press event?

* A. `def onMousePress(mouseX, mouseY):`
* B. `def mouseClick(x, y):`
* C. `onMousePress(mouseX, mouseY):`
* D. `Def onMousePress(mouseX, mouseY):`

---

### **2.**

What will happen when the mouse is pressed in the following code?

```python
c = Circle(200, 200, 30)

def onMousePress(mouseX, mouseY):
    c.centerX = mouseX
    c.centerY = mouseY
```

* A. The circle disappears
* B. The circle moves to where the mouse is clicked
* C. A new circle is created
* D. Nothing happens

---

### **3.**

If the mouse is clicked at (150, 200), where will the circle be drawn?

```python
def onMousePress(mouseX, mouseY):
    Circle(mouseX + 50, mouseY, 20)
```

* A. (100, 200)
* B. (150, 150)
* C. (200, 200)
* D. (150, 250)

---

<div class="break"></div>

### **4.**

Which event runs continuously many times per second?

* A. `onMousePress`
* B. `onMouseMove`
* C. `onStep`
* D. `onKeyPress`

---

### **5.**

Which of the following is a valid variable name?

* A. `my circle`
* B. `2circle`
* C. `circle1`
* D. `def`

---

### **6.**

What will this code do after one step?

```python
ball = Circle(200, 200, 20)
ball.speedX = 5

def onStep():
    ball.centerX += ball.speedX
```

* A. Move the ball left
* B. Move the ball right
* C. Move the ball up
* D. Do nothing

---

### **7.**

What is `speedX` in the code above?

* A. A built-in Python keyword
* B. A custom property
* C. A function
* D. An event handler

---

<div class="break"></div>

### **8.**

What will happen after 3 steps?

```python
ball = Circle(200, 200, 20)
ball.speedY = 10

def onStep():
    ball.centerY += ball.speedY
```

* A. The ball moves to 230
* B. The ball moves to 220
* C. The ball moves to 210
* D. The ball moves to 240

---

### **9.**

Which event should you use to make something follow the mouse smoothly?

* A. `onStep`
* B. `onMousePress`
* C. `onMouseMove`
* D. `onKeyPress`

---

### **10.**

What will this code do?

```python
c = Circle(200, 200, 20)
c.color = 'red'

def onMousePress(mouseX, mouseY):
    c.fill = c.color
```

* A. The circle turns red when clicked
* B. The circle moves
* C. The circle disappears
* D. Nothing happens

---

<div class="break"></div>

# **Answer Key**

1. A
2. B
3. C
4. C
5. C
6. B
7. B
8. A
9. C
10. A
