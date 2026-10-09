<div class="title">
    <h1>
        Unit 2 Practice Test       
    </h1>
    <div class="print-on">
        <strong>Name:</strong>&nbsp;<span>&nbsp;</span>
    </div>
</div>

## Arduino Programming

## Multiple Choice

### 1.

What is the purpose of the `setup()` function in an Arduino program?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong>It runs repeatedly while the Arduino is operating.</td>
<td><strong>B. </strong>It runs once when the Arduino starts or resets.</td>
</tr>
<tr>
<td><strong>C. </strong>It only reads analog sensors.</td>
<td><strong>D. </strong>It controls the Arduino's power supply.</td>
</tr>
</table>

### 2.

What is the purpose of the `loop()` function?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong>It runs repeatedly after <span class="answer-code">setup()</span> finishes.</td>
<td><strong>B. </strong>It runs only once when the Arduino starts.</td>
</tr>
<tr>
<td><strong>C. </strong>It defines all of the variables in the program.</td>
<td><strong>D. </strong>It connects the Arduino to the computer.</td>
</tr>
</table>

### 3.

What is the purpose of `pinMode()`?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong>It reads the value of a pin.</td>
<td><strong>B. </strong>It sets a pin to be used as an input or an output.</td>
</tr>
<tr>
<td><strong>C. </strong>It turns an LED on or off.</td>
<td><strong>D. </strong>It changes an analog value into a digital value.</td>
</tr>
</table>

### 4.

Which line correctly sets pin 8 as an output?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong><span class="answer-code">pinMode(8, INPUT);</span></td>
<td><strong>B. </strong><span class="answer-code">pinMode(8, OUTPUT);</span></td>
</tr>
<tr>
<td><strong>C. </strong><span class="answer-code">digitalWrite(8, OUTPUT);</span></td>
<td><strong>D. </strong><span class="answer-code">digitalRead(8, OUTPUT);</span></td>
</tr>
</table>

<div class="break"></div>

### 5.

Which line correctly sets pin 2 as an input for a button?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong><span class="answer-code">pinMode(2, INPUT);</span></td>
<td><strong>B. </strong><span class="answer-code">pinMode(2, OUTPUT);</span></td>
</tr>
<tr>
<td><strong>C. </strong><span class="answer-code">digitalWrite(2, INPUT);</span></td>
<td><strong>D. </strong><span class="answer-code">analogRead(2, INPUT);</span></td>
</tr>
</table>

### 6.

Consider this code:

```cpp
int ledPin = 8;

void setup() {
    pinMode(ledPin, OUTPUT);
}

void loop() {
    digitalWrite(ledPin, HIGH);
    delay(1000);
    digitalWrite(ledPin, LOW);
    delay(1000);
}
```

What will the LED do?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong>Turn on and stay on</td>
<td><strong>B. </strong>Turn on and off repeatedly</td>
</tr>
<tr>
<td><strong>C. </strong>Stay off</td>
<td><strong>D. </strong>Turn on only once and then stop</td>
</tr>
</table>

### 7.

What is the purpose of a variable such as this?

```cpp
int ledPin = 8;
```

<table class="mcq-choices">
<tr>
<td><strong>A. </strong>It gives the name <span class="answer-code">ledPin</span> to the value 8 so the value can be used later in the program.</td>
<td><strong>B. </strong>It automatically turns pin 8 on.</td>
</tr>
<tr>
<td><strong>C. </strong>It sets pin 8 to be an input.</td>
<td><strong>D. </strong>It reads the voltage on pin 8.</td>
</tr>
</table>

<div class="break"></div>

### 8.

Which line reads whether a button connected to pin 2 is HIGH or LOW?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong><span class="answer-code">digitalWrite(2, HIGH);</span></td>
<td><strong>B. </strong><span class="answer-code">digitalRead(2);</span></td>
</tr>
<tr>
<td><strong>C. </strong><span class="answer-code">analogWrite(2, HIGH);</span></td>
<td><strong>D. </strong><span class="answer-code">pinMode(2, HIGH);</span></td>
</tr>
</table>

### 9.

What is wrong with this code?

```cpp
int buttonPin = 2;
int ledPin = 8;

void setup() {
    pinMode(buttonPin, INPUT);
    pinMode(ledPin, INPUT);
}

void loop() {
    int buttonState = digitalRead(buttonPin);

    if (buttonState == HIGH) {
        digitalWrite(ledPin, HIGH);
    }
}
```

<table class="mcq-choices">
<tr>
<td><strong>A. </strong>The button should be an output.</td>
<td><strong>B. </strong>The LED pin should be set as an output, not an input.</td>
</tr>
<tr>
<td><strong>C. </strong><span class="answer-code">digitalRead()</span> cannot be used with buttons.</td>
<td><strong>D. </strong>The variable <span class="answer-code">buttonState</span> should be a <span class="answer-code">double</span>.</td>
</tr>
</table>

<div class="break"></div>

### 10.

Which code will turn an LED on when a button is pressed and off when the button is not pressed?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong><pre class="answer-code-block">if (buttonState == HIGH) {
    digitalWrite(ledPin, HIGH);
} else {
    digitalWrite(ledPin, LOW);
}</pre></td>
<td><strong>B. </strong><pre class="answer-code-block">if (buttonState == HIGH) {
    digitalWrite(ledPin, LOW);
} else {
    digitalWrite(ledPin, HIGH);
}</pre></td>
</tr>
<tr>
<td><strong>C. </strong><pre class="answer-code-block">if (buttonState = HIGH) {
    digitalRead(ledPin);
}</pre></td>
<td><strong>D. </strong><pre class="answer-code-block">if (buttonState == LOW) {
    digitalWrite(ledPin, LOW);
}</pre></td>
</tr>
</table>

### 11.

What is a nested `if` statement?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong>An <span class="answer-code">if</span> statement placed inside another <span class="answer-code">if</span> statement</td>
<td><strong>B. </strong>Two <span class="answer-code">if</span> statements that always run at the same time</td>
</tr>
<tr>
<td><strong>C. </strong>An <span class="answer-code">if</span> statement that repeats forever</td>
<td><strong>D. </strong>An <span class="answer-code">if</span> statement that can only use sensor values</td>
</tr>
</table>

### 12.

A potentiometer is connected to `A0`. Which line would store its analog reading in a variable?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong><span class="answer-code">int potValue = analogRead(A0);</span></td>
<td><strong>B. </strong><span class="answer-code">int potValue = digitalRead(A0);</span></td>
</tr>
<tr>
<td><strong>C. </strong><span class="answer-code">int potValue = analogWrite(A0);</span></td>
<td><strong>D. </strong><span class="answer-code">int potValue = digitalWrite(A0, HIGH);</span></td>
</tr>
</table>

<div class="break"></div>

### 13.

Which statement correctly compares `analogRead()` and `analogWrite()`?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong><span class="answer-code">analogRead()</span> gets a value from an input, while <span class="answer-code">analogWrite()</span> controls an output.</td>
<td><strong>B. </strong><span class="answer-code">analogRead()</span> controls an output, while <span class="answer-code">analogWrite()</span> reads an input.</td>
</tr>
<tr>
<td><strong>C. </strong>Both functions only work with buttons.</td>
<td><strong>D. </strong>Both functions only produce HIGH or LOW.</td>
</tr>
</table>

### 14.

A TMP36 temperature sensor is connected to an analog input. Which function would you use to get the sensor's reading?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong><span class="answer-code">digitalWrite()</span></td>
<td><strong>B. </strong><span class="answer-code">digitalRead()</span></td>
</tr>
<tr>
<td><strong>C. </strong><span class="answer-code">analogRead()</span></td>
<td><strong>D. </strong><span class="answer-code">pinMode()</span></td>
</tr>
</table>

### 15.

An ultrasonic distance sensor sends out a sound pulse and waits for the sound to bounce back. What does the Arduino use this information to determine?

<table class="mcq-choices">
<tr>
<td><strong>A. </strong>The distance to an object</td>
<td><strong>B. </strong>The temperature of an object</td>
</tr>
<tr>
<td><strong>C. </strong>The resistance of an object</td>
<td><strong>D. </strong>The brightness of an object</td>
</tr>
</table>

<div class="print-off">

### Answer Key

<ol class="answer-key">
<li><strong>B</strong></li>
<li><strong>A</strong></li>
<li><strong>B</strong></li>
<li><strong>B</strong></li>
<li><strong>A</strong></li>
<li><strong>B</strong></li>
<li><strong>A</strong></li>
<li><strong>B</strong></li>
<li><strong>B</strong></li>
<li><strong>A</strong></li>
<li><strong>A</strong></li>
<li><strong>A</strong></li>
<li><strong>A</strong></li>
<li><strong>C</strong></li>
<li><strong>A</strong></li>
</ol>

</div>
