# SHOULDER TURRET HUD SYSTEM

Overview
The Shoulder Turret HUD System is a wearable mechatronics prototype designed to replicate head-motion tracking using an IMU sensor (MPU6050) to control a dual-axis servo turret. The system provides directional alignment based on head movement and displays a visual crosshair-based HUD on an OLED display using optical reflection (mirror + magnification lens concept).

This project explores real-time motion tracking, servo stabilization, and wearable human-machine interface design.

---

 Core Concept
- Head movement is captured using MPU6050 (accelerometer + gyroscope)
- Motion data is mapped to servo angles
- Dual-axis turret responds in real-time
- OLED displays crosshair / targeting UI
- Optical system (mirror + lens) creates HUD projection effect

---

 Key Features
- 360° rotational tracking (pan axis)
- Real-time motion response
- Wearable shoulder-mounted design
- Crosshair HUD simulation
- Optical reflection-based display enhancement
- Laser pointer integration (alignment indicator)

---

 System Components
- Arduino UNO (Main controller)
- MPU6050 (Gyro + Accelerometer)
- SG90 / MG996R Servo Motors (Pan & Tilt)
- OLED Display (I2C SSD1306)
- Laser Module
- Mirror + Magnifying Lens (HUD projection system)
- External power supply (for servos)

---

 Working Principle
1. MPU6050 reads head orientation (X/Y/Z rotation)
2. Arduino processes motion data
3. Servo motors replicate angular movement
4. OLED renders a fixed crosshair HUD
5. Optical system overlays HUD into user field of view
6. Laser indicates turret direction

---
System Behavior
- Head rotates → turret follows instantly
- Center position = neutral alignment
- Fast motion smoothing applied via filtering
- OLED crosshair remains fixed reference point

Future Upgrades
- Wireless version (ESP32 upgrade)
- AI-based target prediction
- Head calibration system
- IMU fusion filtering (Kalman Filter)
- Mini camera integration for vision tracking
- Voice control interface
- Gesture override system

## Status
Prototype Phase 1 – Mechanical + Motion Tracking Complete
