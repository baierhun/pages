# Micro Servo — Miuzei MS18 + UNO R4 WiFi

## Wiring

| Servo Wire | Connection |
|---|---|
| Orange/yellow — Signal | D9 |
| Red — Power | External regulated 5V supply (+) |
| Brown — Ground | External supply (−) and Arduino GND |

## Code

```cpp
#include <Servo.h>

Servo myServo;

const int SERVO_PIN = 9;

void setup() {
  myServo.attach(SERVO_PIN);
  myServo.write(90);
}

void loop() {
  myServo.write(45);
  delay(1000);

  myServo.write(90);
  delay(1000);

  myServo.write(135);
  delay(1000);
}
```