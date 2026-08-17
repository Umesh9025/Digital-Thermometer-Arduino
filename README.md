# 🌡️ Digital Thermometer using Arduino

A beginner-friendly digital thermometer project using an Arduino Uno, TMP36 temperature sensor, and 16×2 LCD.

The circuit was designed and tested using Tinkercad Circuits.

## 📌 Project Overview

This project measures temperature using a TMP36 analog temperature sensor and displays the measured temperature on a 16×2 LCD.

The Arduino reads the analog voltage produced by the TMP36 through analog pin A0, converts the ADC reading into voltage, calculates the temperature in Celsius, and displays the result on the LCD.

## 🧰 Components Used

- Arduino Uno
- Breadboard
- TMP36 temperature sensor
- 16×2 LCD
- 10k potentiometer
- 220Ω resistor
- Jumper wires
- Tinkercad Circuits

## 🔌 Circuit Connections

### TMP36

| TMP36 Pin | Arduino |
|---|---|
| Pin 1 | 5V |
| Pin 2 | A0 |
| Pin 3 | GND |

### 16×2 LCD

| LCD Pin | Connection |
|---|---|
| GND | GND |
| VCC | 5V |
| VO | Potentiometer middle pin |
| RS | Digital Pin 7 |
| RW | GND |
| E | Digital Pin 6 |
| DB4 | Digital Pin 5 |
| DB5 | Digital Pin 4 |
| DB6 | Digital Pin 3 |
| DB7 | Digital Pin 2 |
| LED (+) | 5V through 220Ω resistor |
| LED (-) | GND |

## ⚙️ How It Works

The TMP36 produces an analog voltage related to temperature.

The Arduino reads this voltage using its analog-to-digital converter (ADC):

```text
TMP36
  ↓
Analog voltage
  ↓
Arduino A0
  ↓
ADC reading
  ↓
Voltage calculation
  ↓
Temperature calculation
  ↓
16×2 LCD
```
## 📷 Circuit Simulation
![Digital Thermometer Circuit](./OUTPUT%20CIRCUIT.png)
