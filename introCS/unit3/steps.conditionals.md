<div class="title">
    <h1>From Words to Code: Conditionals</h1>
    <div class="print-on">
        <strong>Name:</strong>&nbsp;<span>&nbsp;</span>
    </div>
</div>

Read each sentence, mark its parts, and then translate it into code. A **conditional** lets an action happen only if a condition is true.

### Steps

1. **Box WHEN it happens.** Look for “when the mouse is pressed,” “when the mouse moves,” or “on every step.” If there is no event, write the code outside the event functions.
2. **Underline the shape or its name.** What are you creating or changing?
3. **Circle the action.** Are you drawing, setting a property, moving, or increasing something?
4. **Put parentheses around the details.** Find property names, numbers, colors, positions, and amounts.
5. **Put brackets around the condition.** Look for “if.” What must be true for the action to happen?
6. **Write the code.** Put the action in the correct event function. If there is a condition, indent the action inside the `if` statement.

### Example

“On every step, move the ball 3 pixels right if its center’s x-coordinate is less than 350.”

- **Box:** On every step
- **Underline:** ball
- **Circle:** move
- **Parentheses:** (3 pixels right), (350)
- **Brackets:** [if its center’s x-coordinate is less than 350]

Moving right means increasing `centerX`. “Less than” translates to `<`.

```python
def onStep():
    if ball.centerX < 350:
        ball.centerX += 3
```

The condition is checked every step. The ball moves only when the condition is true.

### Practice

Mark each sentence first. Then write your code in CMU CS Academy. These sentences build one program—use the same ball for all five.

##### 1. Draw a circle named ball centered at (200, 50) with a radius of 20.

##### 2. Give the ball an orange fill and a black border.

##### 3. When the mouse is pressed, make the ball’s center’s x and y coordinates equal to the mouse’s x and y coordinate respectively.

##### 4. On every step, move the ball 2 pixels down if its center’s y-coordinate is less than 350.