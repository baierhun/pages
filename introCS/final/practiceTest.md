# **Intro to CS Practice Exam**

**Name:** ____________________________________

---

# **Multiple Choice**

### **15 Questions**

---

### **1. Which shape is blue only on the left side?** 

A. `Rect(50, 50, 40, 40, fill=gradient('blue', 'white', start='left'))`

B. `Rect(50, 50, 40, 40, fill=gradient('white', 'blue', start='left'))`

C. `Rect(50, 50, 40, 40, fill=gradient('blue', 'white'))`

D. `Rect(50, 50, 40, 40, fill='blue')`

---

### **2. Which line of code is written correctly?** 

A. `Oval(150, 150, 80, 40 fill='purple')`

B. `Oval(150, 150, 80, 40, fill=purple)`

C. `Oval(150, 150, 80, 40, fill='purple')`

D. `Oval(150, 150, 80, 40, 'fill=purple')`

---

### **3. Which of the following is NOT a built-in shape property?** 

A. `opacity`

B. `rotateAngle`

C. `speed`

D. `border`

---

### **4. Which line of code would draw a circle with a black border?** 

A. `Circle(200, 200, 30, border='black')`

B. `Circle(200, 200, 30, fillBorder='black')`

C. `Circle(200, 200, 30, outline='black')`

D. `Circle(200, 200, 30, borderColor='black')`

---

### **5. Which lines of code would draw a dashed vertical line down the center of the canvas?** 

<table class="answer-table">
<tr>

<td>
A.

<pre>
Line(200, 0, 200, 400, dashes=True)
</pre>

</td>

<td>
B.

<pre>
Line(0, 200, 400, 200, dashes=True)
</pre>

</td>

</tr>

<tr>

<td>
C.

<pre>
Line(0, 0, 400, 400, dashes=True)
</pre>

</td>

<td>
D.

<pre>
Line(400, 0, 0, 400, dashes=True)
</pre>

</td>

</tr>
</table>

---

### **6. Which event handler automatically repeats many times every second?** 

A. `onMousePress`

B. `onKeyPress`

C. `onStep`

D. `redrawAll`

---

### **7. Which expression would place a shape 30 units below the mouse?** 

A. `mouseX + 30`

B. `mouseY - 30`

C. `mouseX - 30`

D. `mouseY + 30`

---

### **8. How would you move this shape upward using its speed variable?** 

```python
bird = Circle(300, 300, 20, fill='yellow')
bird.speedY = 8
```

A. `bird.centerY += bird.speedY`

B. `bird.centerX -= bird.speedY`

C. `bird.centerY -= bird.speedY`

D. `bird.speedY += bird.centerY`

---

### **9. Which variable name is valid in Python?** 

A. `2circle`

B. `my circle`

C. `def`

D. `circle2`

---

### **10. How many stars will be created after the mouse is clicked 4 times?** 

```python
def onMousePress(mouseX, mouseY):
    Star(mouseX, mouseY, 25, 5, fill='gold')
```

A. 1

B. 2

C. 4

D. 5

---

### **11. Which line correctly checks if a shape touches a point?** 

A. `if rect.hits(mouseX, mouseY):`

B. `if rect.hitsShape(mouseX, mouseY):`

C. `if rect.hit(mouseX, mouseY):`

D. `if rect.touches(mouseX, mouseY):`

---

### **12. What is wrong with this code?** 

```python
if score > 10
    Label('Winner!', 200, 200)
```

A. `Label` cannot be used in conditionals.

B. The `if` statement is missing a colon.

C. `score` must be in quotes.

D. `>` is not a valid operator.

---

### **13. How many circles will be drawn if the mouse is pressed at `(250, 50)`?** 

```python
def onMousePress(mouseX, mouseY):
    if mouseX > 200:
        Circle(mouseX, mouseY, 20, fill='red')

    if mouseY < 100:
        Circle(mouseX, mouseY, 10, fill='blue')
```

A. 0

B. 1

C. 2

D. 3

---

### **14. Which program moves the circle left only when the left arrow key is pressed?** 

<table class="answer-table">
<tr>

<td>
A.

<pre>
c = Circle(200, 200, 30)

def onKeyPress(key):
    if key == 'left':
        c.centerX -= 50
</pre>

</td>

<td>
B.

<pre>
c = Circle(200, 200, 30)

def onKeyPress(key):
    if key == left:
        c.centerX -= 50
</pre>

</td>

</tr>

<tr>

<td>
C.

<pre>
c = Circle(200, 200, 30)

def onKeyPress(key):
    if key = 'left':
        c.centerX -= 50
</pre>

</td>

<td>
D.

<pre>
c = Circle(200, 200, 30)

def onKeyPress(key):
    if key != 'right':
        c.centerY -= 50
</pre>

</td>

</tr>
</table>

---

<div class="break"></div>

### **15. What will happen when the mouse is pressed?** 

```python
box = Rect(100, 100, 100, 100, fill='green')
msg = Label('', 200, 50)

def onMousePress(mouseX, mouseY):
    if box.hits(mouseX, mouseY):
        msg.value = 'inside'
    else:
        msg.value = 'outside'
```

A. The label will always say `'outside'`

B. The label changes depending on where the mouse is clicked

C. The program has an error

D. The label never changes

---

<div class="break"></div>

# **Matching**

### **Questions 16–25**

Match the terms on the left to the descriptions on the right.

<table class="answer-table" style="width:100%; border-collapse:collapse; table-layout:fixed;border:none !important;">

<colgroup>
  <col style="width:45pt;">
  <col style="width:140pt;">
  <col>
</colgroup>

<tr>
<th style="text-align:center;">#</th>
<th>Term</th>
<th>Description</th>
</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">16.</td>
<td style="border:none !important;height:30pt;"><code>onStep</code></td>
<td style="border:none !important;height:30pt;"><b>A.</b> a gradual blend between colors</td>
</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">17.</td>
<td style="border:none !important;height:30pt;"><code>gradient</code></td>
<td style="border:none !important;height:30pt;"><b>B.</b> a repeating function used for animation</td>
</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">18.</td>
<td style="border:none !important;height:30pt;"><code>Group</code></td>
<td style="border:none !important;height:30pt;"><b>C.</b> horizontal center position of a shape</td>

</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">19.</td>
<td style="border:none !important;height:30pt;"><code>canvas</code></td>
<td style="border:none !important;height:30pt;"><b>D.</b> a boolean property</td>

</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">20.</td>
<td style="border:none !important;height:30pt;"><code>.dashes</code></td>
<td style="border:none !important;height:30pt;"><b>E.</b> determines how much a shape is rotated</td>

</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">21.</td>
<td style="border:none !important;height:30pt;"><code>.centerX</code></td>
<td style="border:none !important;height:30pt;"><b>AB.</b> the area where shapes are displayed</td>

</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">22.</td>
<td style="border:none !important;height:30pt;"><code>variable</code></td>
<td style="border:none !important;height:30pt;"><b>AC.</b> checks whether a shape touches another shape</td>

</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">23.</td>
<td style="border:none !important;height:30pt;"><code>.rotateAngle</code></td>
<td style="border:none !important;height:30pt;"><b>AD.</b> statements that compare values to decide what code runs</td>

</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">24.</td>
<td style="border:none !important;height:30pt;"><code>.hitsShape(shape)</code></td>
<td style="border:none !important;height:30pt;"><b>AE.</b> a named object used to store information</td>

</tr>

<tr>
<td style="text-align:center;border:none !important;height:30pt;">25.</td>
<td style="border:none !important;height:30pt;"><code>conditionals</code></td>

<td style="border:none !important;height:30pt;"><b>ABC.</b> a collection of multiple shapes stored together</td>
</tr>

</table>

---

<div class="break"></div>

# **Short Answer**

### **3 Questions**

---

### **26.** 
Describe a situation where someone misuses a computer or program in a way that would be considered unethical. Explain why the action is wrong. 

<div class="spacer" style="--scale: 13.5;"></div>

---

### **27.** 
You receive a text message saying you won a free gaming console. The message includes a suspicious link.

Explain **three ways** you could determine whether this message is safe or dangerous. 

<div class="spacer" style="--scale: 20.5;"></div>
<div class="break"></div>

### **28.** 
Explain the dangers of sharing too much personal information online. What are ways to protect yourself? 

<div class="spacer" style="--scale: 20.5;"></div>

# **Answers**

| MC | Matching |
| :--- | :--- |
| 1. A | 16. B |
| 2. C | 17. A |
| 3. C | 18. ABC |
| 4. A | 19. AB |
| 5. A | 20. D |
| 6. C | 21. C |
| 7. D | 22. AE |
| 8. C | 23. E |
| 9. D | 24. AC |
| 10. C | 25. AD |
| 11. A |  |
| 12. B |  |
| 13. C |  |
| 14. A |  |
| 15. B |  |