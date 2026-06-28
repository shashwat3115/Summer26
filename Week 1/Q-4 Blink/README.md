# LED Blink Project

## Overview

The **LED Blink** project is a beginner Arduino application that demonstrates how to control a digital output pin. The LED connected to **digital pin 13** blinks continuously at a fixed interval, introducing the basics of Arduino programming, digital outputs, and timing functions.

---

## Hardware Required

- Arduino UNO
- USB Type-A to Type-B cable
- LED (optional, if not using the onboard LED)
- 220 Ω resistor (for an external LED)
- Breadboard (optional)
- Jumper wires (optional)

---

## Circuit Diagram Description

### Using the Onboard LED

No external wiring is required. The Arduino UNO has a built-in LED connected to **digital pin 13**.

### Using an External LED

```text
Arduino UNO

D13 ---- 220Ω Resistor ----> LED ----> GND
```

- Connect the LED anode (+) to **D13** through a **220 Ω resistor**.
- Connect the LED cathode (-) to **GND**.

---

## How to Upload Code

1. Connect the Arduino UNO to your computer using a USB cable.
2. Open the Arduino IDE.
3. Open the `led_blink.ino` sketch.
4. Go to **Tools → Board** and select **Arduino UNO**.
5. Go to **Tools → Port** and select the correct COM port.
6. Click the **Verify** button to compile the sketch.
7. Click the **Upload** button.
8. Wait until the message **"Done uploading."** appears.

---

## Expected Output

- The LED connected to **digital pin 13** blinks continuously.
- The LED stays **ON for 500 ms** and **OFF for 500 ms**.
- If using the enhanced versions:
  - The Serial Monitor displays the blink count.
  - A potentiometer connected to **A0** adjusts the blink speed.

---

## Troubleshooting Tips

1. **LED does not blink**
   - Check that the correct board and COM port are selected.
   - Verify the LED polarity and resistor connections if using an external LED.

2. **Upload fails**
   - Ensure the USB cable supports data transfer.
   - Close the Serial Monitor before uploading.
   - Press the RESET button on the Arduino and try uploading again.

3. **No Serial Monitor output**
   - Set the Serial Monitor baud rate to **9600**.
   - Verify that `Serial.begin(9600);` is included in the sketch.

4. **Potentiometer does not change blink speed**
   - Confirm that the potentiometer is connected to **5V**, **GND**, and **A0**.
   - Check for loose wires or incorrect connections.

---

## Project Structure

```text
week1/
└── led_blink/
    ├── led_blink.ino
    └── README.md
```

---

## Author

**Name:** Shashwat Singh

**Course:** IoT Summer School 2026

**Week:** Week 1 – LED Blink Project

**License:** MIT License
