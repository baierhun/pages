<div class="title">
    <h1>
        Unit 3 Project: Connected Boards
    </h1>
    <div class="print-on">
        <strong>Name:</strong>&nbsp;<span>&nbsp;</span>
    </div>
</div>

## Submission - Each Student

Submit as a PDF on Canvas (I will not accept shared Google Docs):

- Your Arduino code.
- A brief reflection explaining:
  - How your board sends and receives data.
  - One problem you encountered and how you solved it.
  - Your contribution to the project.

## Your Challenge

Work with a partner to build a connected system using two Arduino boards. Each board must read two inputs and control two outputs.

Your inputs must control your partner’s outputs, and your partner’s inputs must control yours. Use MQTT and Home Assistant to send and receive the data.

Choose a purpose for your system and explain how its inputs and outputs work together.

## Requirements for Each Student

### Two Inputs

- At least one input must be an **ultrasonic sensor** or an **IR transmitter/receiver setup** used to detect something.
- The IR transmitter and receiver together count as **one input setup**.
- Choose your second input.

### Two Outputs

- One output must be the **onboard LED matrix**.
- Choose your second output.

### Communication

- Publish data from both inputs.
- Subscribe to the messages needed to control both outputs.
- Each input must control a different output on your partner’s board.
- Both outputs must respond to your partner’s inputs.
- Both boards must send and receive data while the project is running.

Your partnership needs **four inputs and four outputs total**.

## Plan Your Connections

Complete this table before building. Describe the exact trigger and response.

For example: “When the distance is less than 15 cm, display a warning symbol on my partner’s LED matrix.”

<table style="width:100%; border-collapse:collapse; font-size:0.9rem;">
    <thead>
        <tr>
            <th style="border:1px solid #ccc; padding:4px 6px; text-align:left;">Input</th>
            <th style="border:1px solid #ccc; padding:4px 6px; text-align:left;">Output on Partner’s Board</th>
            <th style="border:1px solid #ccc; padding:4px 6px; text-align:left;">Trigger and Response</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="border:1px solid #ccc; padding:4px 6px;">Student A — Input 1:</td>
            <td style="border:1px solid #ccc; padding:4px 6px;">Student B — Output 1:</td>
            <td style="border:1px solid #ccc; padding:4px 6px;"></td>
        </tr>
        <tr>
            <td style="border:1px solid #ccc; padding:4px 6px;">Student A — Input 2:</td>
            <td style="border:1px solid #ccc; padding:4px 6px;">Student B — Output 2:</td>
            <td style="border:1px solid #ccc; padding:4px 6px;"></td>
        </tr>
        <tr>
            <td style="border:1px solid #ccc; padding:4px 6px;">Student B — Input 1:</td>
            <td style="border:1px solid #ccc; padding:4px 6px;">Student A — Output 1:</td>
            <td style="border:1px solid #ccc; padding:4px 6px;"></td>
        </tr>
        <tr>
            <td style="border:1px solid #ccc; padding:4px 6px;">Student B — Input 2:</td>
            <td style="border:1px solid #ccc; padding:4px 6px;">Student A — Output 2:</td>
            <td style="border:1px solid #ccc; padding:4px 6px;"></td>
        </tr>
    </tbody>
</table>

For each connection, record:

- The MQTT topic.
- The message or values being sent.
- What the receiving board should do.

## Build and Test

1. Test each input and output on your own board.
2. Agree on MQTT topics, message values, and what each received message should do.
3. Connect the boards through MQTT and Home Assistant.
4. Test all four input-to-output connections.
5. Test repeated triggers and changes back to the normal state. Decide what happens when a button is released, an object moves away, or a sensor reading changes.

## Demonstrate and Submit

### Together

- Demonstrate all four connections.
- Explain your system’s purpose and how the two boards work together.

## Success Criteria

- Each board has two inputs and two outputs.
- Each student meets the required sensor and output choices.
- All four cross-board connections work reliably.
- Both boards send and receive data.
- Both students can explain their own wiring and code.