# Ultrasonic Sensor — UNO R4 WiFi

## Wiring

* Vcc and Gnd pins go to 5v and Ground respectively on the Arduino
* Trig and echo pins go to pins 9 and 8 respectively on hte Arduino

## Code

```cpp
#include <SmartEngineering.h>

const int triggerPin = 9;
const int echoPin = 8;

UltrasonicSensor sensor(triggerPin, echoPin); // TRIG, ECHO

void setup() {
  Serial.begin(115200);
  sensor.begin();
}

void loop() {
    float distance = sensor.distanceCm();
    Serial.println(distance);
  }
}
```