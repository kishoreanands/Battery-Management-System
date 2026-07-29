# 🔋 Battery Management System (BMS) for Electric Vehicles

> An intelligent Battery Management System (BMS) designed for Electric Vehicles (EVs) that improves battery safety, efficiency, and reliability through automatic temperature control, dual-battery management, real-time voltage monitoring, and intelligent battery switching.

---

## 📖 Project Overview

The **Battery Management System (BMS)** is an Electric Vehicle (EV)-based project developed to improve battery performance, ensure operational safety, and provide uninterrupted power to the vehicle.

The system uses **two rechargeable batteries**, where one battery powers the vehicle while the other battery is charged through a dedicated charging mechanism. During vehicle operation, **four DC motors** are incorporated as part of the project's charging concept to provide electrical energy for charging the secondary battery. Once the charging battery reaches its predefined voltage level, the Arduino automatically switches the batteries, ensuring continuous vehicle operation.

To protect the batteries from overheating, the system continuously monitors battery temperature using a temperature sensor. If the temperature exceeds the safe operating limit, a cooling fan is automatically activated until the battery temperature returns to a safe level.

The system also provides real-time monitoring of:

* 🌡️ Battery Temperature
* 🔋 Battery 1 Voltage
* 🔋 Battery 2 Voltage
* ⚡ Charging Voltage
* 🔄 Active Battery Status
* 🌀 Cooling Fan Status

---

# 🎯 Objectives

* Develop a smart Battery Management System for Electric Vehicles.
* Monitor battery temperature continuously.
* Prevent battery overheating using an automatic cooling fan.
* Automatically switch between two batteries.
* Monitor battery voltages in real time.
* Display charging voltage generated during vehicle operation.
* Improve battery efficiency and lifespan.
* Ensure uninterrupted vehicle power.

---

# ✨ Key Features

* 🌡️ Real-Time Temperature Monitoring
* 🌀 Automatic Cooling Fan Control
* 🔋 Dual Battery Management
* 🔄 Automatic Battery Switching
* ⚡ Charging Voltage Monitoring
* 📊 Battery Voltage Monitoring
* 🚗 Four DC Motor-Based Charging Mechanism
* 📟 Live System Status Monitoring
* 🛡️ Battery Protection Against Overheating

---

# ⚙️ System Working

### Step 1 – Vehicle Startup

* Battery 1 supplies power to the electric vehicle.
* Battery 2 remains connected to the charging circuit.

### Step 2 – Charging Process

* Four DC motors operate as part of the vehicle system.
* The generated electrical energy is supplied to the charging circuit to charge the secondary battery.

### Step 3 – Temperature Monitoring

* The LM35 temperature sensor continuously monitors battery temperature.
* If the temperature exceeds the predefined threshold:

  * Cooling fan turns ON automatically.
* When the temperature drops to a safe level:

  * Cooling fan turns OFF automatically.

### Step 4 – Voltage Monitoring

The Arduino continuously monitors:

* Battery 1 Voltage
* Battery 2 Voltage
* Charging Voltage
* Active Battery
* Charging Battery

### Step 5 – Automatic Battery Switching

* Battery 1 powers the vehicle while Battery 2 charges.
* Once Battery 2 reaches full charge, the Arduino switches the power source.
* Battery 2 begins powering the vehicle.
* Battery 1 starts charging.
* This process continues automatically throughout vehicle operation.

---

# 🔋 Battery Management Process

| Battery Status          | Operation           |
| ----------------------- | ------------------- |
| Battery 1               | Powers the Vehicle  |
| Battery 2               | Charging            |
| Battery 2 Fully Charged | Automatic Switching |
| Battery 2               | Powers the Vehicle  |
| Battery 1               | Charging            |

---

# 🌡️ Temperature Protection

The system continuously checks battery temperature.

| Temperature     | Fan Status |
| --------------- | ---------- |
| Below Threshold | OFF        |
| Above Threshold | ON         |

This automatic cooling mechanism protects the battery pack from overheating and improves battery life.

---

# ⚡ Monitoring Parameters

The system continuously displays:

* Battery Temperature
* Battery 1 Voltage
* Battery 2 Voltage
* Charging Voltage
* Active Battery
* Charging Battery
* Cooling Fan Status

---

# 🛠 Hardware Components

* Arduino Uno / Nano
* LM35 Temperature Sensor
* Four DC Motors
* Two Rechargeable Batteries
* Dual Relay Module
* Cooling Fan
* Battery Voltage Sensors
* Charging Voltage Sensor
* Battery Management Circuit (BMS)
* Charging Circuit
* Motor Driver Module
* EV Chassis

---

# 💻 Software

* Arduino IDE
* Embedded C (Arduino Programming)
* Serial Monitor

---

# 🏗 System Architecture

```text
                 Temperature Sensor
                         │
                         ▼
                 Arduino Controller
                         │
      ┌──────────────────┼──────────────────┐
      │                  │                  │
      ▼                  ▼                  ▼
 Cooling Fan     Voltage Monitoring    Relay Module
                         │
                         ▼
        ┌──────────────────────────────────┐
        │      Battery Management Unit     │
        └───────────────┬──────────────────┘
                        │
          ┌─────────────┴─────────────┐
          ▼                           ▼
     Battery 1                   Battery 2
   (Power Source)              (Charging)
          │                           ▲
          └─────────────┬─────────────┘
                        │
                Charging Circuit
                        ▲
                        │
               Four DC Motors
                        │
                        ▼
              Electric Vehicle Drive
```

---

# 🚗 Applications

* Electric Vehicles
* Electric Bikes
* Electric Scooters
* Smart Battery Systems
* Renewable Energy Systems
* Educational EV Projects

---

# ✅ Advantages

* Automatic battery switching
* Continuous charging
* Temperature protection
* Improved battery life
* Better energy utilization
* Reliable vehicle operation
* Low maintenance
* Real-time monitoring
* Enhanced battery safety

---

# 🚀 Future Enhancements

* IoT-Based Remote Monitoring
* Mobile Application
* Bluetooth/Wi-Fi Connectivity
* LCD/OLED Display
* GPS Integration
* Battery Health Prediction
* State of Charge (SOC) Monitoring
* State of Health (SOH) Analysis
* Cloud Data Logging
* Regenerative Braking Integration

---

# 👨‍💻 Project Outcome

The Battery Management System demonstrates an intelligent and efficient approach to EV battery management by integrating automatic temperature control, dual-battery switching, voltage monitoring, and charging management into a single system.

The project enhances battery safety, improves operational efficiency, and ensures continuous power delivery, making it a practical solution for educational and prototype Electric Vehicle applications.

---

## 📄 License

This project is developed for **academic and educational purposes** and can be extended for future research and Electric Vehicle innovations.
