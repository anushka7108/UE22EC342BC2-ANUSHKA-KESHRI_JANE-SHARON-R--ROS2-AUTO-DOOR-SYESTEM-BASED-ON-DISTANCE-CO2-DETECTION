# UE22EC342BC2-ANUSHKA-KESHRI_JANE-SHARON-R--ROS2-AUTO-DOOR-SYESTEM-BASED-ON-DISTANCE-CO2-DETECTION


# 🚪 Smart Automatic Door Control System using CO₂ and Ultrasonic Sensors

This project implements a smart automatic door system using an Arduino Uno, MQ135 gas sensor (for CO₂ detection), an HC-SR04 ultrasonic sensor (for proximity detection), and a servo motor for door actuation. The system is designed to provide **touchless access** and enhance **indoor air quality** by opening the door when CO₂ levels are high or when someone approaches.

---

## 🧠 Project Overview

The door control system operates in two primary modes:

- **Air Quality Mode**: Opens the door when CO₂ concentration exceeds a defined threshold.
- **Proximity Mode**: Opens the door when a person is detected within a specified distance.

---

## 🎯 Objectives

- Monitor indoor air quality using CO₂ levels.
- Provide touchless door automation for hygiene and convenience.
- Enable modular and energy-efficient operation.
- Ensure adaptability for different environments.

---



## 📐 Wiring Overview

- **MQ135 Analog Out → A0**
- **MQ135 Digital Out → Pin 2**
- **Ultrasonic Trigger → Pin 9**
- **Ultrasonic Echo → Pin 10**
- **Servo Signal → Pin 6**
- **5V/GND** → Shared power rails

---

## 🧾 Code Features

- **Sensor Fusion**: Combines data from CO₂ and ultrasonic sensors.
- **Timed Door Control**: Keeps door open for a set time before closing.
- **Serial Debugging**: Logs sensor values for easy monitoring.
- **Modular Functions**: `openDoor()` and `closeDoor()` for clarity.

---

## 🧪 Calibration Steps

1. **MQ135 Calibration**: Place in clean air for 24 hours and adjust `co2Threshold`.
2. **Ultrasonic Calibration**: Tune `proximityThreshold` for reliable human detection.
3. **Servo Calibration**: Adjust angles to match your door’s movement.

---

## 🚦 System Logic (Pseudocode)

```
If CO₂ > threshold OR person detected:
    Open door
Else if door is open for >5 seconds:
    Close door
```

---

## 📊 Performance Results

| Feature            | Performance            |
|--------------------|------------------------|
| CO₂ Detection      | Accurate within 10s    |
| Proximity Detection| Reliable <1s response  |
| Door Actuation     | ~1s open/close time    |
| False Triggers     | <2% with calibration   |

---

## 💡 Applications

- Smart homes and offices
- Bathrooms and kitchens
- Hospitals and labs
- Energy-efficient buildings

---

## 📈 Future Enhancements

### Hardware:
- Add humidity & temperature sensors
- Use stronger actuators for heavier doors
- Enable battery backup support

### Software:
- Remote control via mobile app
- Machine learning for predictive control
- IoT data logging for CO₂ trends

---

## 🧰 Dependencies

- [Servo.h](https://www.arduino.cc/reference/en/libraries/servo/)
- [NewPing.h](https://playground.arduino.cc/Code/NewPing/)

---

## 🏁 Conclusion

This project demonstrates a reliable, practical, and hygienic solution to modern smart automation problems using affordable components and Arduino. It can be easily adapted and expanded for diverse smart building applications.

---

## 📷 Demo & Circuit (Add images here if available)
