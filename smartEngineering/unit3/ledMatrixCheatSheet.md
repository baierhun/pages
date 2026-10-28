# Onboard LED Matrix — UNO R4 WiFi

## Wiring

No wiring needed. The matrix is built into the board.

## Code

```cpp
#include "Arduino_LED_Matrix.h"

ArduinoLEDMatrix matrix;

// 1 = LED on, 0 = LED off
uint8_t picture[8][12] = {
  {0,0,0,0,0,0,0,0,0,0,0,0},
  {0,0,0,1,1,0,0,1,1,0,0,0},
  {0,0,0,1,1,0,0,1,1,0,0,0},
  {0,0,0,0,0,0,0,0,0,0,0,0},
  {0,0,1,0,0,0,0,0,0,1,0,0},
  {0,0,0,1,0,0,0,0,1,0,0,0},
  {0,0,0,0,1,1,1,1,0,0,0,0},
  {0,0,0,0,0,0,0,0,0,0,0,0}
};

void setup() {
  matrix.begin();
  matrix.renderBitmap(picture, 8, 12);
}

void loop() {
}
```