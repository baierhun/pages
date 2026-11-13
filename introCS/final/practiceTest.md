<style>
.answer-key-horizontal {
display: flex;
flex-wrap: wrap;
gap: 8px 28px;
padding-left: 28px;
}
.answer-key-horizontal li {
margin: 0;
min-width: 45px;
}
</style>

<div class="title">
<h1>Intro to CS Practice Exam</h1>
<div class="print-on">
<strong>Name:</strong>&nbsp;<span>&nbsp;</span>
</div>
</div>

## Multiple Choice

Choose the best answer for each question.

##### 1. Which shape is blue only on the left side?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">Rect(50, 50, 40, 40, fill=gradient('blue', 'white', start='left'))</span></td>
<td><strong>B.</strong> <span class="answer-code">Rect(50, 50, 40, 40, fill=gradient('white', 'blue', start='left'))</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">Rect(50, 50, 40, 40, fill=gradient('blue', 'white'))</span></td>
<td><strong>D.</strong> <span class="answer-code">Rect(50, 50, 40, 40, fill='blue')</span></td>
</tr>
</table>

##### 2. Which line of code is written correctly?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">Oval(150, 150, 80, 40 fill='purple')</span></td>
<td><strong>B.</strong> <span class="answer-code">Oval(150, 150, 80, 40, fill=purple)</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">Oval(150, 150, 80, 40, fill='purple')</span></td>
<td><strong>D.</strong> <span class="answer-code">Oval(150, 150, 80, 40, 'fill=purple')</span></td>
</tr>
</table>

##### 3. Which of the following is NOT a built-in shape property?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">opacity</span></td>
<td><strong>B.</strong> <span class="answer-code">rotateAngle</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">speed</span></td>
<td><strong>D.</strong> <span class="answer-code">border</span></td>
</tr>
</table>

##### 4. Which line of code would draw a circle with a black border?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">Circle(200, 200, 30, border='black')</span></td>
<td><strong>B.</strong> <span class="answer-code">Circle(200, 200, 30, fillBorder='black')</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">Circle(200, 200, 30, outline='black')</span></td>
<td><strong>D.</strong> <span class="answer-code">Circle(200, 200, 30, borderColor='black')</span></td>
</tr>
</table>

<div class="break"></div>

##### 5. Which line of code would draw a dashed vertical line down the center of the canvas?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">Line(200, 0, 200, 400, dashes=True)</span></td>
<td><strong>B.</strong> <span class="answer-code">Line(0, 200, 400, 200, dashes=True)</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">Line(0, 0, 400, 400, dashes=True)</span></td>
<td><strong>D.</strong> <span class="answer-code">Line(400, 0, 0, 400, dashes=True)</span></td>
</tr>
</table>

##### 6. Which event handler automatically repeats many times every second?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">onMousePress</span></td>
<td><strong>B.</strong> <span class="answer-code">onKeyPress</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">onStep</span></td>
<td><strong>D.</strong> <span class="answer-code">redrawAll</span></td>
</tr>
</table>

##### 7. Which expression would place a shape 30 units below the mouse?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">mouseX + 30</span></td>
<td><strong>B.</strong> <span class="answer-code">mouseY - 30</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">mouseX - 30</span></td>
<td><strong>D.</strong> <span class="answer-code">mouseY + 30</span></td>
</tr>
</table>

##### 8. How would you move this shape upward using its speed variable?

```python
bird = Circle(300, 300, 20, fill='yellow')
bird.speedY = 8
```

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">bird.centerY += bird.speedY</span></td>
<td><strong>B.</strong> <span class="answer-code">bird.centerX -= bird.speedY</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">bird.centerY -= bird.speedY</span></td>
<td><strong>D.</strong> <span class="answer-code">bird.speedY += bird.centerY</span></td>
</tr>
</table>

##### 9. Which variable name is valid in Python?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">2circle</span></td>
<td><strong>B.</strong> <span class="answer-code">my circle</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">def</span></td>
<td><strong>D.</strong> <span class="answer-code">circle2</span></td>
</tr>
</table>

<div class="break"></div>

##### 10. How many stars will be created after the mouse is clicked 4 times?

```python
def onMousePress(mouseX, mouseY):
    Star(mouseX, mouseY, 25, 5, fill='gold')
```

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">1</span></td>
<td><strong>B.</strong> <span class="answer-code">2</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">4</span></td>
<td><strong>D.</strong> <span class="answer-code">5</span></td>
</tr>
</table>

##### 11. Which line correctly checks if a shape touches a point?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">if rect.hits(mouseX, mouseY):</span></td>
<td><strong>B.</strong> <span class="answer-code">if rect.hitsShape(mouseX, mouseY):</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">if rect.hit(mouseX, mouseY):</span></td>
<td><strong>D.</strong> <span class="answer-code">if rect.touches(mouseX, mouseY):</span></td>
</tr>
</table>

##### 12. What is wrong with this code?

```python
if score > 10
    Label('Winner!', 200, 200)
```

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">Label</span> cannot be used in conditionals.</td>
<td><strong>B.</strong> The <span class="answer-code">if</span> statement is missing a colon.</td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">score</span> must be in quotes.</td>
<td><strong>D.</strong> <span class="answer-code">&gt;</span> is not a valid operator.</td>
</tr>
</table>

##### 13. How many circles will be drawn if the mouse is pressed at `(250, 50)`?

```python
def onMousePress(mouseX, mouseY):
    if mouseX > 200:
        Circle(mouseX, mouseY, 20, fill='red')

    if mouseY < 100:
        Circle(mouseX, mouseY, 10, fill='blue')
```

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> <span class="answer-code">0</span></td>
<td><strong>B.</strong> <span class="answer-code">1</span></td>
</tr>
<tr>
<td><strong>C.</strong> <span class="answer-code">2</span></td>
<td><strong>D.</strong> <span class="answer-code">3</span></td>
</tr>
</table>

<div class="break"></div>

##### 14. Which program moves the circle left only when the left arrow key is pressed?

<table class="mcq-choices">
<tr>
<td><strong>A.</strong><br><span class="answer-code">c = Circle(200, 200, 30)<br>def onKeyPress(key):<br>&nbsp;&nbsp;&nbsp;&nbsp;if key == 'left':<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c.centerX -= 50</span></td>
<td><strong>B.</strong><br><span class="answer-code">c = Circle(200, 200, 30)<br>def onKeyPress(key):<br>&nbsp;&nbsp;&nbsp;&nbsp;if key == left:<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c.centerX -= 50</span></td>
</tr>
<tr>
<td><strong>C.</strong><br><span class="answer-code">c = Circle(200, 200, 30)<br>def onKeyPress(key):<br>&nbsp;&nbsp;&nbsp;&nbsp;if key = 'left':<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c.centerX -= 50</span></td>
<td><strong>D.</strong><br><span class="answer-code">c = Circle(200, 200, 30)<br>def onKeyPress(key):<br>&nbsp;&nbsp;&nbsp;&nbsp;if key != 'right':<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c.centerY -= 50</span></td>
</tr>
</table>

##### 15. What will happen when the mouse is pressed?

```python
box = Rect(100, 100, 100, 100, fill='green')
msg = Label('', 200, 50)

def onMousePress(mouseX, mouseY):
    if box.hits(mouseX, mouseY):
        msg.value = 'inside'
    else:
        msg.value = 'outside'
```

<table class="mcq-choices">
<tr>
<td><strong>A.</strong> The label will always say <span class="answer-code">'outside'</span>.</td>
<td><strong>B.</strong> The label changes depending on where the mouse is clicked.</td>
</tr>
<tr>
<td><strong>C.</strong> The program has an error.</td>
<td><strong>D.</strong> The label never changes.</td>
</tr>
</table>

<div class="break"></div>

## Matching

Match each term on the left to a description on the right. Questions 16–25.

<table class="answer-table" style="width:100%; border-collapse:collapse; table-layout:fixed; border:none !important;">
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
<td style="text-align:center; border:none !important; height:30pt;">16.</td>
<td style="border:none !important; height:30pt;"><code>onStep</code></td>
<td style="border:none !important; height:30pt;"><strong>A.</strong> a gradual blend between colors</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">17.</td>
<td style="border:none !important; height:30pt;"><code>gradient</code></td>
<td style="border:none !important; height:30pt;"><strong>B.</strong> a repeating function used for animation</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">18.</td>
<td style="border:none !important; height:30pt;"><code>Group</code></td>
<td style="border:none !important; height:30pt;"><strong>C.</strong> horizontal center position of a shape</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">19.</td>
<td style="border:none !important; height:30pt;"><code>canvas</code></td>
<td style="border:none !important; height:30pt;"><strong>D.</strong> a boolean property</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">20.</td>
<td style="border:none !important; height:30pt;"><code>.dashes</code></td>
<td style="border:none !important; height:30pt;"><strong>E.</strong> determines how much a shape is rotated</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">21.</td>
<td style="border:none !important; height:30pt;"><code>.centerX</code></td>
<td style="border:none !important; height:30pt;"><strong>AB.</strong> the area where shapes are displayed</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">22.</td>
<td style="border:none !important; height:30pt;"><code>variable</code></td>
<td style="border:none !important; height:30pt;"><strong>AC.</strong> checks whether a shape touches another shape</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">23.</td>
<td style="border:none !important; height:30pt;"><code>.rotateAngle</code></td>
<td style="border:none !important; height:30pt;"><strong>AD.</strong> statements that compare values to decide what code runs</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">24.</td>
<td style="border:none !important; height:30pt;"><code>.hitsShape(shape)</code></td>
<td style="border:none !important; height:30pt;"><strong>AE.</strong> a named object used to store information</td>
</tr>
<tr>
<td style="text-align:center; border:none !important; height:30pt;">25.</td>
<td style="border:none !important; height:30pt;"><code>conditionals</code></td>
<td style="border:none !important; height:30pt;"><strong>ABC.</strong> a collection of multiple shapes stored together</td>
</tr>
</table>
<div class="break"></div>

## Short Answer

### 26.
Describe a situation where someone misuses a computer or program in a way that would be considered unethical. Explain why the action is wrong.

<div class="spacer" style="--scale: 13.5;"></div>

### 27.
You receive a text message saying you won a free gaming console. The message includes a suspicious link.

Explain **three ways** you could determine whether this message is safe or dangerous.

<div class="spacer" style="--scale: 20.5;"></div>
<div class="break"></div>

### 28.
Explain the dangers of sharing too much personal information online. What are ways to protect yourself?

<div class="spacer" style="--scale: 40.5;"></div>

<h3>Answer Key</h3>
<ol class="answer-key answer-key-horizontal">
<li><strong>A</strong></li>
<li><strong>C</strong></li>
<li><strong>C</strong></li>
<li><strong>A</strong></li>
<li><strong>A</strong></li>
<li><strong>C</strong></li>
<li><strong>D</strong></li>
<li><strong>C</strong></li>
<li><strong>D</strong></li>
<li><strong>C</strong></li>
<li><strong>A</strong></li>
<li><strong>B</strong></li>
<li><strong>C</strong></li>
<li><strong>A</strong></li>
<li><strong>B</strong></li>
<li><strong>B</strong></li>
<li><strong>A</strong></li>
<li><strong>ABC</strong></li>
<li><strong>AB</strong></li>
<li><strong>D</strong></li>
<li><strong>C</strong></li>
<li><strong>AE</strong></li>
<li><strong>E</strong></li>
<li><strong>AC</strong></li>
<li><strong>AD</strong></li>
</ol>
