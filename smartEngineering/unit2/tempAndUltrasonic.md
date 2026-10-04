##### Temperature Sensor

```c++
// Looking at the flat side
// left pin is +5V
// middle pin is analog signal
// right pin is -GND

int TEMP_PIN = A0;

void setup()
{
  pinMode(TEMP_PIN, INPUT);
  Serial.begin(9600);
}

void loop()
{
  // reads in a value between 0-1023
  int temp_in = analogRead(TEMP_PIN);
  // converts input to a voltage reading
  double temp_voltage = temp_in * 5.0/1024.0;
  // converts voltage to degrees celsius.
  double temp = (temp_voltage - 0.5)*100;
  Serial.println(temp);
  delay(100);
}
```

##### Ultrasonic Sensor

```c++
// VCC pin is +5V
// Trig pin (trigger) tells the transmitter when to start transmitting
// Echo pin reads in from the receiver 

// Define HC-SR04 Pin Connections
const int TRIG_PIN = 9;
const int ECHO_PIN = 8;

void setup() {
  // Initialize serial communication for printing distance
  Serial.begin(9600);

  // Set pin modes
  pinMode(TRIG_PIN, OUTPUT);
  pinMode(ECHO_PIN, INPUT);
}

void loop() {
  // 1. Clear the trigger pin to ensure a clean HIGH pulse
  digitalWrite(TRIG_PIN, LOW);
  delayMicroseconds(2);

  // 2. Trigger the sensor by sending a 10-microsecond HIGH pulse
  digitalWrite(TRIG_PIN, HIGH);
  delayMicroseconds(10);
  digitalWrite(TRIG_PIN, LOW);

  // 3. Read the echo pin; pulseIn returns the sound wave travel time in microseconds
  long duration = pulseIn(ECHO_PIN, HIGH);

  // 4. Calculate distance in centimeters:
  // Speed of sound = ~0.034 cm/us. Sound travels to target and back, so divide by 2.
  float distanceCm = (duration * 0.0343) / 2;

  // 5. Print the result to the Serial Monitor
  Serial.print("Distance: ");
  Serial.print(distanceCm);
  Serial.println(" cm");

  // Wait 100ms before taking another reading
  delay(100);
}
```