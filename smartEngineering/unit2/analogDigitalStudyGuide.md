# Arduino Study Guide: Inputs and Outputs

## 1. Digital Read and Digital Write

**Digital** means there are only two possible states:

* **HIGH** = ______ V
* **LOW** = ______ V

### `digitalRead()`

`digitalRead()` is used to **read** a digital ______ from a pin.

A digital input can be:

* HIGH
* 

Example:

```cpp
int buttonState = digitalRead(2);
```

This reads the value from pin ______ and stores it in `buttonState`.

**Think:** `digitalRead()` = Arduino is ______ something.

---

### `digitalWrite()`

`digitalWrite()` is used to ______ a digital output pin HIGH or LOW.

Example:

```cpp
digitalWrite(13, HIGH);
```

This sets pin 13 to ______.

Example:

```cpp
digitalWrite(13, LOW);
```

This sets pin 13 to ______.

**Think:** `digitalWrite()` = Arduino is ______ something.

<div class="break"></div>

## 2. LEDs

An LED is a component that produces ______ when current flows through it.

An LED has two legs:

* **Anode** = ______ leg
* **Cathode** = ______ leg

The LED should normally be connected with a ______ resistor to limit the current.

A typical LED circuit looks like:

```text
Arduino pin → resistor → LED → GND
```

The LED turns on when the Arduino pin is set to:

**HIGH / LOW**

The LED turns off when the Arduino pin is set to:

**HIGH / LOW**

### Important

Current needs a complete ______ for the LED to work.

---

## 3. Push Buttons

A push button is an example of a digital ______.

The Arduino can use `digitalRead()` to determine whether the button is pressed.

For example:

```cpp
int button = digitalRead(2);
```

The Arduino is reading pin ______.

A common button circuit uses:

* 5V
* a button
* a ______ resistor
* GND
* an Arduino input pin

<div class="break"></div>

## 4. Pull-Down Resistors

A pull-down resistor makes sure an input has a known value when the button is ______.

Without a pull-down resistor, the input can be **floating**, which means the Arduino may read unpredictable ______ and ______ values.

A pull-down resistor connects the input pin to:

**5V / GND**

When the button is not pressed, the input reads:

**HIGH / LOW**

When the button is pressed, the input reads:

**HIGH / LOW**

### Remember

**Pull-down → pulls the input toward ______.**

---

## 5. Analog Read

Unlike a digital input, an analog input can measure a ______ range of values.

`analogRead()` is commonly used with sensors and a ______.

Example:

```cpp
int value = analogRead(A0);
```

This reads the analog value from pin ______.

On many Arduino boards, `analogRead()` returns a value from:

**0 to ______**

A reading of 0 represents approximately ______ volts.

A reading near the maximum represents approximately ______ volts.

**Think:** `analogRead()` = Arduino is ______ a variable voltage.

<div class="break"></div>

## 6. Potentiometers

A potentiometer is a variable ______.

Turning the knob changes the resistance and therefore changes the ______ at the middle pin.

The Arduino can use `analogRead()` to measure this changing voltage.

Example:

```cpp
int value = analogRead(A0);
```

If you turn the potentiometer, the value returned by `analogRead()` should ______.

## 7. Analog Write

`analogWrite()` is used to control the ______ of an output.

On many Arduino boards, `analogWrite()` uses a technique called ______ to rapidly turn a digital signal on and off.

The value used with `analogWrite()` is commonly from:

**0 to ______**

Example:

```cpp
analogWrite(9, 255);
```

This produces the ______ output level. For example:

```cpp
analogWrite(9, 0);
```

This produces the ______ output level.

A value between 0 and 255 produces an output somewhere ______.

### LED Brightness

For an LED:

```cpp
analogWrite(9, 50);
```

would make the LED ______ than:

```cpp
analogWrite(9, 200);
```

<div class="break"></div>

## 8. Digital vs. Analog

Complete the table.

| Function         | Reads/Writes | Type       | Example       |
| ---------------- | ------------ | ---------- | ------------- |
| `digitalRead()`  | ______       | Digital    | Button        |
| `digitalWrite()` | ______       | Digital    | LED           |
| `analogRead()`   | ______       | Analog     | Potentiometer |
| `analogWrite()`  | ______       | PWM output | LED           |

### Easy way to remember

**Read = Arduino gets information.**

**Write = Arduino ______ information.**

**Digital = ______ choices.**

**Analog = a ______ range of values.**

---

## 9. Passive Buzzers

A **passive buzzer** needs a rapidly changing electrical signal to produce a ______.

Unlike an active buzzer, a passive buzzer can produce different ______.

The Arduino can use the `tone()` function to play a frequency.

Example:

```cpp
tone(8, 440);
```

This plays a tone on pin ______ at a frequency of ______ Hz.

A higher frequency produces a ______ pitch.

A lower frequency produces a ______ pitch.

To stop the tone:

```cpp
noTone(8);
```

The number `8` tells Arduino which ______ the buzzer is connected to.

<div class="break"></div>

## 10. Key Vocabulary

Fill in each blank.

**Digital:** Has ______ possible states.

**HIGH:** Approximately ______ V.

**LOW:** Approximately ______ V.

**Input:** Something the Arduino ______.

**Output:** Something the Arduino ______.

**LED:** Produces ______.

**Push button:** A digital ______.

**Pull-down resistor:** Connects an input toward ______.

**Potentiometer:** A variable ______.

**PWM:** Rapidly switches an output ______ and ______ to simulate different output levels.

**Passive buzzer:** Can produce different ______.

**Frequency:** Measured in ______ and determines the pitch of a buzzer.

---

## Quick Review

1. Which function reads a button?
   `________________________`

2. Which function turns an LED on or off?
   `________________________`

3. Which function reads a potentiometer?
   `________________________`

4. Which function can control LED brightness?
   `________________________`

5. Why does a button circuit need a pull-down resistor?
   `____________________________________________`

6. Where does a pull-down resistor connect the input?
   `____________________________________________`

7. What happens to the analog reading when you turn a potentiometer?
   `____________________________________________`

8. What does `tone(8, 440)` do?
   `____________________________________________`

9. What happens to the pitch when frequency increases?
   `____________________________________________`

10. Why does an LED need a resistor?
    `____________________________________________`
