Here are the **two additional rules** integrated cleanly into the existing guide so they fit naturally with your style and the way you teach the course.

---

# **Unit 1 — Python Style Guide: Spacing and Line Breaks**

This guide explains how to write your Python code neatly so it is easy to read and understand.

## **1. One Command Per Line**

Write each command on its own line.

**Good:**

```python
Circle(100, 100, 50)
Star(20, 40, 30, 60)
```

**Not good:**

```python
Circle(100, 100, 50) Star(20, 40, 30, 60)
```

---

## **2. Put a Space After Each Comma**

When you write something with commas, put **one space** after every comma.

**Good:**

```python
Circle(100, 150, 40, fill='blue')
```

**Not good:**

```python
Circle(100,150,40,fill='blue')
```

---

## **3. No Extra Spaces Before Parentheses**

There should **not** be a space before the parenthesis.

**Good:**

```python
Star(50, 60, 100, 30)
```

**Not good:**

```python
Star (50, 60, 100, 30)
```

---

## **4. Use Blank Lines to Separate Sections**

You can use **one blank line** to make parts of your code easier to see.

**Example:**

```python
# Sun
Star(200, 295, 25, 200, fill='sandybrown')
Star(200, 295, 18, 200, fill=gradient('white', 'yellow'))

# Islands
Oval(40, 330, 30, 90, fill=rgb(50, 25, 19))
Oval(20, 330, 50, 100, fill=rgb(75, 50, 19))
```

---

## **5. Comments**

When you write a comment, put **one space** after the `#`.

**Good:**

```python
# Draw the sun
Circle(300, 50, 40, fill='yellow')
```

**Not good:**

```python
#Draw the sun
Circle(300, 50, 40, fill='yellow')
```

---

# **Unit 2 — Variables, Groups, and Mouse Events Style Guide**

In Unit 2, we begin organizing our programs with **variables**, **groups**, and **mouse event handlers**.

## **1. Put Variable Definitions Near the Top**

Variables that store shapes should usually appear **near the top of your program** so they are easy to find.

**Example:**

```python
player = Circle(200, 200, 20, fill='blue')
enemy = Rect(300, 200, 40, 40, fill='red')
coin = Circle(150, 250, 10, fill='gold')
```

---

## **2. Use Clear Variable Names**

Variable names should describe what the shape represents.

**Good:**

```python
player = Circle(200, 200, 20)
sun = Circle(300, 50, 40)
```

**Not good:**

```python
c = Circle(200, 200, 20)
x = Circle(300, 50, 40)
```

---

## **3. Use Snake Case for Variable Names**

Python variable names use **snake case**, where words are separated with underscores.

**Good:**

```python
player_circle = Circle(200, 200, 20)
enemy_ship = Rect(100, 50, 60, 30)
```

**Not good:**

```python
playerCircle = Circle(200, 200, 20)
EnemyShip = Rect(100, 50, 60, 30)
```

---

## **4. Groups Should Be Stored in a Variable**

When you create a `Group`, assign it to a variable.

Shapes in the group can be **created directly** or **use existing shape variables**.

**Example (creating shapes inside the group):**

```python
car = Group(
    Rect(100, 200, 120, 30),
    Circle(120, 230, 15),
    Circle(200, 230, 15)
)
```

**Example (using existing shapes):**

```python
wheel_left = Circle(120, 230, 15)
wheel_right = Circle(200, 230, 15)
body = Rect(100, 200, 120, 30)

car = Group(body, wheel_left, wheel_right)
```

---

## **5. Break Long Groups Onto Multiple Lines**

If a group has many shapes, put each shape on its own line.

```python
tree = Group(
    Rect(190, 260, 20, 60, fill='brown'),
    Circle(200, 230, 40, fill='green'),
    Circle(170, 240, 30, fill='green'),
    Circle(230, 240, 30, fill='green')
)
```

---

## **6. Leave a Blank Line Before Event Handlers**

Mouse event handlers should be visually separated from the rest of your code.

```python
player = Circle(200, 200, 20, fill='blue')


def onMouseMove(mouseX, mouseY):
    player.centerX = mouseX
    player.centerY = mouseY
```

---

## **7. Indent Code Inside Event Handlers**

All code inside a mouse event handler must be **indented one level**.

**Good:**

```python
def onMousePress(mouseX, mouseY):
    player.centerX = mouseX
```

**Not good:**

```python
def onMousePress(mouseX, mouseY):
player.centerX = mouseX
```

---

# **Unit 3 — Conditionals, Keyboard Events, and Collision Style Guide**

In Unit 3, programs begin to react to conditions, keyboard input, and collisions between shapes.

## **1. Put Spaces Around Comparison Operators**

Put spaces around operators like `==`, `<`, and `>`.

**Good:**

```python
if player.centerX > 300:
    player.centerX = 300
```

**Not good:**

```python
if player.centerX>300:
    player.centerX=300
```

---

## **2. Be Consistent With Parentheses in Conditions**

Conditions may use **parentheses or not**, but be consistent.

**Example:**

```python
if player.centerX > 300:
    player.centerX = 300
```

or

```python
if (player.centerX > 300):
    player.centerX = 300
```

---

## **3. `if` and `else` Should Be Clearly Aligned**

The `else` should line up with the `if`.

**Good:**

```python
if player.hits(enemy):
    enemy.opacity = 0
else:
    player.fill = 'blue'
```

**Not good:**

```python
if player.hits(enemy):
    enemy.opacity = 0
    else:
        player.fill = 'blue'
```

---

## **4. Event Handlers Should Be Near the Bottom**

Keyboard and mouse event handlers should usually appear **near the bottom of your program**.

```python
player = Circle(200, 200, 20, fill='blue')


def onKeyPress(key):
    if key == 'left':
        player.centerX -= 10
```

---

## **5. Use Clear Collision Checks**

Keep collision checks simple and readable.

```python
if player.hits(enemy):
    enemy.opacity = 0
```

or

```python
if player.hitsShape(coin):
    coin.fill = 'gold'
```

---

## **6. Keep Conditions Simple**

Write conditions so they are easy to read.

**Good:**

```python
if player.centerX > 400:
    player.centerX = 400
```

**Not good:**

```python
if(player.centerX>400):
    player.centerX=400
```
