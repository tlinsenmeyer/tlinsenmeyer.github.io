---
title: "SIM‑1 Digital Twin"
description: "A full‑physics HVAC digital twin for testing real control logic, coil dynamics, and system behavior."
layout: default
---

<nav>
  <ul>
    <li><a href="index.md">Home</a></li>
    <li><a href="about.md">About Me</a></li>
    <li><a href="projects.md">Projects</a></li>
    <li><a href="contact.md">Contact</a></li>
  </ul>
</nav>

<p align="center">
  <img src="banner.png" alt="Portfolio Banner" width="100%" />
</p>

---

# SIM‑1 Digital Twin  
*A physics‑based HVAC simulation environment for testing real control logic.*

SIM‑1 is a digital twin of a real air‑handling unit (AHU) designed to simulate HVAC behavior with engineering accuracy. It allows safe testing of control logic, coil dynamics, freeze protection, humidity control, and system interactions without risking real equipment.

This project blends **mechanical engineering**, **control systems**, and **data science** into one unified system.

---

# 🎯 Project Goals

SIM‑1 was built to:

- Model HVAC equipment using **real physics**, not approximations  
- Test **Plain English control logic** (Schneider Electric) in a safe environment  
- Validate coil behavior, valve response, and freeze‑stat protection  
- Provide realistic telemetry for machine learning and analytics  
- Serve as a foundation for future digital twin and BAS optimization work  

---

# 🧱 System Architecture

SIM‑1 is structured into modular subsystems:

<p align="center">
  <img src="Sim1 Architecture.png" alt="SIM‑1 Architecture Diagram" width="90%" />
</p>


### **1. AHUModel (Physics Engine)**
Simulates:

- Coil heat transfer (UA model)  
- Valve Cv behavior  
- Steam humidifier dynamics  
- Fan heat  
- Psychrometrics (enthalpy, humidity ratio, dewpoint)  
- 100% outside air (no mixed air)  

### **2. AHUEngine (Control Logic Runner)**
Executes translated Plain English logic:

- Cooling loop  
- Preheat loop  
- Humidifier loop  
- Freeze protection  
- Mode switching (HEAT / COOL)  

### **3. Trend Logging**
Generates EBO‑style logs:

- Temperatures  
- Valve positions  
- Humidity  
- Coil leaving air conditions  
- Freeze‑stat behavior  

### **4. Simulation Loop**
Runs timestep‑based updates:

- Physics → Control → Physics → Control  
- Adjustable timestep for stability  

---

# 🔧 Engineering Diagram (Described)

**AHU Flow Path:**

