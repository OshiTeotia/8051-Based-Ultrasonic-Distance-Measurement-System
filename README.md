# Ultrasonic Distance Measurement System using 8051 Microcontroller

This project demonstrates a distance measurement system built around the **AT89C51 microcontroller** (8051 family) and the **HC-SR04 ultrasonic sensor**. The system calculates the distance to an obstacle using the time-of-flight of ultrasonic waves and displays the output in centimeters on a **16x2 LCD**. 

This project was implemented as part of an academic exploration in **embedded systems and real-time sensor interfacing**.

---

## 🧭 Project Summary

- **Microcontroller**: AT89C51 (8051 family)
- **Sensor**: HC-SR04 ultrasonic sensor
- **Display**: 16x2 character LCD (HD44780)
- **Language**: Embedded C (Keil µVision)
- **Core Functionality**: Real-time measurement of distance (2 cm to 400 cm)
- **Application**: Object detection, proximity alert systems, automation

---

## 🛠️ Features

- Real-time distance display on LCD in centimeters
- Timer-based pulse duration measurement using 8051 Timer0
- Configurable for short and mid-range object detection
- Stable operation using regulated 5V power supply

---

## ⚙️ Hardware Components

| Component             | Description                            |
|-----------------------|----------------------------------------|
| AT89C51               | 8051-based microcontroller              |
| HC-SR04               | Ultrasonic sensor for distance sensing  |
| 16x2 LCD              | HD44780 controller-based character LCD |
| Crystal Oscillator    | 11.0592 MHz for accurate timing         |
| 7805 Regulator        | +5V power supply                        |
| Resistors, Capacitors | Standard passive components            |
| Breadboard / PCB      | For assembly and testing                |

---

## 💻 Software Tools

- **IDE**: Keil µVision (Embedded C programming)
- **Programmer**: USBasp or equivalent 8051 burner
- **Simulation (optional)**: Proteus or similar

---

## 🔬 Working Principle

1. **Trigger Pulse**: The 8051 sends a 10 µs HIGH signal to the HC-SR04's TRIG pin.
2. **Echo Response**: The sensor emits an ultrasonic burst and sets the ECHO pin HIGH while waiting for the reflection.
3. **Timer Capture**: The 8051 uses Timer0 to measure the duration for which the ECHO pin remains HIGH.
4. **Distance Calculation**: Based on the speed of sound, the microcontroller computes:

### Video Demonstration

You can download and watch the video demonstration here:

[▶️ Download Demo Video](https://photos.app.goo.gl/fRQTp8YLnAbMwUR76)

## Author

**Oshi Teotia**  
B.Tech – Electronics & Communication Engineering  
Nirma University

- GitHub: [@OshiTeotia](https://github.com/OshiTeotia)  
- LinkedIn: [Oshi Teotia](https://www.linkedin.com/in/oshi-teotia)



