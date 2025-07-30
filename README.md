# 🌈 Mood Light - Arduino Project

The **Mood Light** is an interactive Arduino-based lighting system that reacts to ambient light levels in a room. Using a single photoresistor, the project reads the light levels in the room its in and acordingly adjusts the colors of the **two RGB LEDs** to create a soothing and dynamic lighting effect. As the room gets darker or brighter, the RGB LEDs smoothly transition through different color combinations to match the mood of the space.

---

## 🛠️ Components Used

- 1 × Arduino Uno (or compatible board)
- 1 × Photoresistor (LDR)
- 2 × Common Cathode RGB LEDs
- 12 × Jumper Wires
- 7 × 220 Ohm Resistors *(not 20 Ohms — 220Ω is standard for LEDs)*
- 1 × Breadboard
- 1 × USB cable for Arduino

---

## 🔧 How It Works

1. The **photoresistor** detects ambient light intensity and sends an analog signal to the Arduino.
2. The Arduino maps this signal to control the **red**, **green**, and **blue** channels of both **RGB LEDs**.
3. As light levels change (e.g. lights turn off, sunset, etc.), the Arduino dynamically adjusts LED colors:
   - Brighter light may produce cool or vibrant tones.
   - Dimmer environments may trigger warmer or softer colors.
4. The RGB LEDs mix colors via **PWM (pulse-width modulation)** on the Arduino's analog output pins.
5. The system runs continuously, creating a live "mood" response to the room's lighting.

---

## 🖼️ Circuit Overview

- Each RGB LED uses **three 220Ω resistors** to protect the red, green, and blue pins.
- The **photoresistor** is part of a voltage divider with a resistor (~10kΩ) and is connected to an analog input pin (e.g. A0).
- The RGB LEDs are connected to PWM-compatible pins for smooth color transitions (e.g. 9, 10, 11).

---

##  Getting Started

1. Wire up your components according to the included photo
2. Upload the Arduino sketch that reads the light value and maps it to RGB output.
3. Power your Arduino and observe how the LEDs change based on the light in the room.
4. Try covering the photoresistor with your hand or shining a flashlight to see immediate effects.

---

## 🎨 Customize It!

You can personalize your Mood Light by:
- Adjusting color mapping for different lighting moods.
- Adding more LEDs or diffusers.
- Integrating motion or sound sensors for extra interactivity.

---

Feel free to improve or remix the project to suit your goals and most impottantly injoy.
