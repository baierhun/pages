# 🌐 Smart Engineering Final Project: Connected Classroom

## Overview

For your final project, you will build an Arduino system that connects with **four different classmates** through MQTT.

Your board will have **two inputs and two outputs**:

- **One analog input** and **one digital input**.
- **The onboard LED matrix** and **one additional output device**.

Each input will trigger an output on another student’s board. Each output will respond to an input from another student’s board.

**Every connection must involve a unique student.** You will send data to two classmates and receive data from two other classmates, for a total of **four different people**.

Your teacher will manage the Raspberry Pi and provide the Wi-Fi and MQTT connection information. You are responsible for wiring your components, programming your board, and publishing and listening to the correct topics.

## Submission

Make a copy of <a href="https://docs.google.com/document/d/1Xl-Bf6AbDqTXmTq0F0C_bJg3Pu67Ml28Nyc4SM2QRNQ/edit?usp=sharing" target="_blank">this Google document</a>, complete it, save it as a PDF, and submit it to Canvas. In it be sure to include:

1. **Your completed connection table.**
2. **Your final Arduino code**, with comments identifying your inputs, outputs, and MQTT topics. Replace passwords with placeholders before submitting.
3. **A photo of your completed board and wiring.**
4. **A short reflection:**
   - Describe one problem you encountered and how you solved it.
   - Explain how you confirmed that messages reached the correct board.
   - Describe one improvement you would make with more time.

## Requirements

### 1. Two Inputs: One Analog and One Digital

Connect and program:

- **One analog input**, such as a potentiometer or a light sensor wired as an analog input.
- **One digital input**, such as a push button or a switch.

For each input:

- Decide what action or condition will trigger a message.
- Publish a message to the agreed-upon MQTT topic.
- Have that message trigger an output on another student’s board.

Your two inputs must trigger outputs belonging to **two different students**.

### 2. Two Outputs: LED Matrix and One Other Device

Program these two outputs:

- **The onboard LED matrix:** It must change between **at least two different pictures** in response to messages from another student’s input. A blank screen does not count as a picture.
- **One additional output device:** Choose a device such as an external LED, buzzer, or servo.

For each output:

- Subscribe to the agreed-upon MQTT topic.
- Read messages published by another student’s board.
- Make your output respond appropriately.

Your two outputs must receive triggers from **two different students**, and neither student can be someone you send data to.

### 3. Four Unique Connections

Plan this and complete the table in the project worksheet before building. Coordinate with your classmates so everyone agrees on the topics, messages, and responses.

**All four names in the Classmate column must be different.**

Topic names must match exactly between the board publishing the message and the board listening for it. Agree on the message contents, too—for example, whether a trigger sends `ON`, `1`, or a sensor reading.

## Build and Test

1. Choose your analog input, digital input, and additional output device.
2. Design at least two different pictures for the onboard LED matrix.
3. Arrange your four connections and complete the planning table.
4. Wire and test each component.
5. Connect your board using these credentials.
   ```cpp
   const char WIFI_NAME[] = "Programming_Guest";
   const char WIFI_PASSWORD[] = "C$C1a$sHun";
   const char MQTT_SERVER[] = "pif.local";
   const char MQTT_USER[] = "mqttuser";
   const char MQTT_PASSWORD[] = "mqttuser";
   const char CLIENT_ID[] = "arduino-pif-2"; // Unique per board
   ```
6. Program your board to publish and listen to the agreed-upon topics.
7. Test each connection with the appropriate classmate.
8. Test your complete system with all four components connected and the same program running.

Your program must continue checking for incoming messages while monitoring your inputs. All four connections must work without changing or uploading a different program.

## Final Demonstration

Be ready to demonstrate:

- Your analog input triggering a classmate’s output.
- Your digital input triggering a different classmate’s output.
- Your onboard LED matrix changing between at least two pictures in response to a third classmate’s input.
- Your additional output responding to a fourth classmate’s input.

You must also be able to explain:

- How your components are wired.
- What makes one of your inputs analog and the other digital.
- Which topics your board publishes to and listens to.
- What messages your board sends and receives.
- How your code turns those messages into output responses.

You are responsible for your own wiring and code. Coordinate testing with your classmates and help troubleshoot shared connections.
