# IR Transmitter/Receiver — UNO R4 WiFi

## Wiring

For a bare **IR LED transmitter** and **phototransistor receiver**. Check the receiver’s datasheet for collector/emitter identification; leg lengths vary.

| Component | Connection |
|---|---|
| IR LED anode (+, usually longer leg) | D7 through a **1 kΩ resistor** |
| IR LED cathode (−, usually shorter leg) | GND |
| Receiver collector | A0 |
| Receiver emitter | GND |
| **10 kΩ resistor** | Between A0 and 5V |

Point the transmitter toward the receiver. Lower readings mean more received IR.

## Code

```cpp
const int IR_TX_PIN = 7;
const int IR_RX_PIN = A0;

void setup() {
  Serial.begin(9600);
  analogReadResolution(10);

  pinMode(IR_TX_PIN, OUTPUT);
  digitalWrite(IR_TX_PIN, HIGH);
}

void loop() {
  int irValue = analogRead(IR_RX_PIN);

  Serial.print("IR reading: ");
  Serial.println(irValue);

  delay(100);
}
```