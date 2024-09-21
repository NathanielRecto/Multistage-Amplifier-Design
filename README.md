# Multistage BJT Amplifier Design
This project involved designing and analyzing a multistage BJT (Bipolar Junction Transistor) amplifier. The design aimed to meet specific requirements, with analysis and testing carried out using Multisim. Hand calculations for the design are included and a 3-stage (CE-CC-CE) amplifier circuit was used. 
## Objectives: 
The primary goal was to design a BJT amplifier that meets the following specifications:
- **Power Supply:** +10V relative to ground.
- **Quiescent Current:** No larger than 10 mA.
- **No-load Voltage Gain:** |Avo| = 50 (± 10%) at 1 kHz.
- **Maximum No-load Output Voltage Swing:** No smaller than 8 V peak-to-peak at 1 kHz.
- **Loaded Voltage Gain:** At least 90% of the no-load gain (with RL = 1 kΩ).
- **Maximum Loaded Output Voltage Swing:** No smaller than 4 V peak-to-peak (with RL = 1 kΩ).
- **Input Resistance:** No smaller than 20 kΩ at 1 kHz.
- **Amplifier Type:** Inverting or Non-inverting.
- **Frequency Response:** 20 Hz to 50 kHz (−3dB response).
- **Number of Transistor Stages:** Maximum 3.
- **Resistor Values:** Smaller than 220 kΩ (from E24 series).
- **Capacitor Values:** 0.1 μF to 220 μF (selected from specified values).
- **Other Components:** Only BJTs, diodes, and Zener diodes from the ELE404 lab kit.
- **Output Voltage:** Must be free of distortions (e.g., clipping) under all test conditions.
- **Source Resistance (Rs):** 600 Ω under all test conditions.
## Design Process:
A 3-stage amplifier design was made to achieve the required 50 dB gain with input resistance greater than 20kΩ. The design included:
- Two CE (Common Emitter) stages with equal voltage gains.
- One CC (Common Collector) stage to buffer the output and stabilize the circuit.
The design used Multisim for simulation and DC sweep analysis to generate characteristic graphs. The circuit was optimized for low collector current (400 μA) in the CE stages, keeping the design power-efficient while meeting the gain and performance requirements. Each stage’s biasing resistors were calculated using Kirchhoff's Current Law (KCL) and the transistor's operating points.
## Components
- **BJTs:** 2N3904 (3 units)
- **Resistors:**
  - **Biasing Resistors:** R1 = 91 kΩ, R2 = 68 kΩ, etc.
  - **Collector Resistors:** RC1 = 15 kΩ, RC2 = 13 kΩ, etc.
- **Capacitors:** C1 = 10 μF, C2 = 100 μF, etc.
- **Coupling Capacitors:** Selected based on the input resistance and frequency response requirements.
- **Power Supply:** +10V DC.
## Multisim Schematic Circuit
![circuit](https://github.com/user-attachments/assets/e3c7bb1b-de0b-4ccd-8217-3db64fbf2322)
## Circuit Testing:
The amplifier circuit was simulated and tested in Multisim. These measurements include:
1. **Voltage Gain:**
    - **No-load gain:** 49.21 V/V
    - **Loaded gain:** 44.31 V/V with RL = 1kΩ
2. **Output Voltage Swing:**
    - **No-load:** 4.81 V peak-to-peak
    - **Loaded:** 4.32 V peak-to-peak
3. **Input Resistance:** Calculated at 32.25 kΩ
4. **Frequency Response:** Measured to meet the 20 Hz to 50 KHz bandwidth requirement
## Experimental Results:
The final circuit was tested under different loading conditions, and the results were compared to the design specifications. 
Key results:
- **Quiescent Current:** 5.12 mA (well within the 10 mA limit).
- **No-load Gain:** 49.21 V/V (within 10% of the 50 V/V requirement).
- **Maximum Output Voltage Swing:** Below the required 8 V peak-to-peak, but all other key specifications were met with minimal error percentages.
## Conclusion
Despite a discrepancy in the maximum no-load output voltage swing, the design met all other critical specifications, including voltage gain, input resistance, and frequency response. The minor errors were attributed to the approximations made during hand calculations and simulation assumptions. Overall, the 3-stage BJT amplifier successfully demonstrated the principles of multistage amplifier design.
