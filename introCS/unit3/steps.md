<div class="title">
    <h1>From Words to Code</h1>
    <div class="print-on">
        <strong>Name:</strong>&nbsp;<span>&nbsp;</span>
    </div>
</div>

Read each sentence, mark its parts, and then translate it into code.

### Steps

1. **Box WHEN it happens.** Look for “when the mouse is pressed,” “when the mouse moves,” or “on every step.” This tells you which event function to use. If there is no event, write the code outside the event functions.
2. **Underline the shape or its name.** What are you creating or changing?
3. **Circle the action.** Are you drawing, setting a property, moving, or increasing something?
4. **Put parentheses around the details.** Find property names, numbers, colors, positions, and amounts.
5. **Write the code.** Put the action in the correct place and use the details to complete it.

### Example

“On every step, move the ball 2 pixels down.”

- **Box:** On every step
- **Underline:** ball
- **Circle:** move
- **Parentheses:** (2 pixels down)

Moving down means increasing the ball’s `centerY` by 2.

```python
def onStep():
    ball.centerY += 2
```

### Practice

Mark each sentence first. Then write your code in the sandbox on CS Academy. These sentences build one program—use the same ball for all five.

##### 1. Draw a circle named ball centered at (200, 200) with a radius of 25.

##### 2. Give the ball a purple fill and a black border.

##### 3. When the mouse is pressed, move the ball’s center to the mouse’s position.

##### 4. When the mouse moves, make the ball’s radius equal to the mouse’s x-coordinate divided by 10, plus 5.

##### 5. On every step, move the ball 2 pixels down.