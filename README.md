# Mosquito-sensor

Prototype for mosquito detection using motor-simulated wing vibration, IR/ultrasonic sensors, and signal processing with MATLAB/Embedded C.

## Project Overview
Mosquitoes spread diseases like dengue, malaria, and chikungunya. This project explores low-cost methods for **detecting mosquito presence and species identification** by analyzing wing vibrations.

Two main approaches are studied:
- **Light interaction**: Using IR/photoelectric sensors to capture wingbeat frequencies.
- **Sound interaction**: Simulating mosquito wing sounds and analyzing them with signal processing.
- The goal of this project is to explore **low-cost and low-power methods** to detect mosquitoes based on their flying characteristics (wing vibrations, optical reflections, ultrasonic interactions).  
- This prototype focuses first on **light-based detection** before extending to ultrasonic simulations.

## Objectives
1. Control and vary motor speed to simulate mosquito wing frequencies (< 1000 Hz).
2. Capture reflected light/signal from wings and body using different wavelengths.
3. Analyze signals for species-specific characteristics.
4. Explore ultrasonic simulation inspired by bat echolocation.
5. Develop a low-cost, low-power prototype.

## Approach & Methodology

### 1. Motor-Simulated Wing Vibration
- A **small DC motor with attached wings** is used to simulate mosquito wing flapping.  
- Speed is controlled via **power supply** or **potentiometer** (later with a microcontroller).  
- An Oscilloscope used to verify that the sensor signal corresponds to the wing rotation speed.  

### 2. Optical Interaction (Light Sensors & LEDs)
- Place a light sensor in front of the rotating wings to capture reflected signals.  
- Initial test: use normal light and check if signal variations can be detected.  
- Next step: use **two LEDs at different wavelengths**:
  - One wavelength for mosquito body reflection.  
  - Another wavelength for wing reflection.  
- Goal: Differentiate body vs wing reflections → add information for species identification.  

### 3. Ultrasonic Interaction (Future Work)
- Initial step: simulate ultrasonic detection in MATLAB to test feasibility.
- Implement microcontroller-based motor control and automated frequency analysis.
- Extend detection using ultrasonic sensing for enhanced accuracy. 

## Current Progress(as of october 2025)
-  Built initial prototype: motor + potentiometer for speed control.  
-  Tested basic optical setup with sensor and an oscilloscope.  
-  Next: integrate dual-wavelength LED system.

## 📸 Prototype Images
(Back view):  
![Test1](testimage1.jpg)

Frontside wiring with motor and potentiometer:  
![Test2](2ndtestimage.jpg)

## Hardware Components
- DC motor with custom wing attachment (to simulate mosquito wing flapping)
- Potentiometer (motor speed control)
- IR emitter and photodiode / photoelectric sensor
- Optional: Ultrasonic transducer
- Breadboard / PCB prototype
- Power supply (low voltage, low consumption)

## Software & Tools
- **Embedded C** for microcontroller firmware
- **MATLAB/Simulink** for signal processing & visualization
- **TINA-TI** for analog circuit simulation
- An Oscilloscope for real-time signal validation


