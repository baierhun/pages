# Ultrasonic Sensor — HC-SR04 + UNO R4 WiFi

## Wiring

| Sensor Pin | Arduino Pin |
|---|---|
| VCC | 5V |
| GND | GND |
| TRIG | D7 |
| ECHO | D8 |

## Code

```cpp
const int TRIG_PIN = 7;
const int ECHO_PIN = 8;

void setup() {
  Serial.begin(9600);
  pinMode(TRIG_PIN, OUTPUT);
  pinMode(ECHO_PIN, INPUT);
  digitalWrite(TRIG_PIN, LOW);
}

void loop() {
  digitalWrite(TRIG_PIN, LOW);
  delayMicroseconds(2);
  digitalWrite(TRIG_PIN, HIGH);
  delayMicroseconds(10);
  digitalWrite(TRIG_PIN, LOW);

  unsigned long duration = pulseIn(ECHO_PIN, HIGH, 30000UL);

  if (duration == 0) {
    Serial.println("No echo detected");
  } else {
    float distanceCm = duration / 58.0;

    Serial.print("Distance: ");
    Serial.print(distanceCm, 1);
    Serial.println(" cm");
  }

  delay(100);
}
```