# DC-DC Boost Converter Simulation using LTspice

## Overview

This project demonstrates the design and simulation of a DC-DC Boost Converter in LTspice. A Boost Converter is a power electronic circuit used to increase a lower DC input voltage to a higher DC output voltage. In this simulation, a 12V DC input supply is boosted to approximately 24V DC using high-frequency switching and energy storage elements.

## Circuit Diagram

<img src="circuit.png" alt="Boost Converter Circuit" width="700">

## Output Waveform

<img src="waveform.png" alt="Boost Converter Output Waveform" width="700">

## Components Used

- Input Voltage Source (V1) = 12V
- NMOS Transistor (BSZ0905NS)
- Schottky Diode (MBRS140)
- Inductor (L1) = 470 µH
- Capacitor (C1) = 22 µF
- Load Resistor (R1) = 24 Ω
- PWM Pulse Source (V2)

## Simulation Parameters

- Switching Frequency = 100 kHz
- Duty Cycle = 50%
- Transient Analysis = 10 ms

## Working Principle

The PWM signal drives the MOSFET, causing it to switch ON and OFF at a high frequency. When the MOSFET is ON, current flows through the inductor and energy is stored in its magnetic field. When the MOSFET turns OFF, the stored energy in the inductor is released through the Schottky diode to the output capacitor and load. The capacitor smooths the output voltage and reduces ripple, resulting in a DC output voltage higher than the input voltage.

## Results

The simulation shows the output voltage increasing from 0V during startup and settling around 22V–24V. This verifies the boost converter operation, where the output voltage is greater than the 12V input supply. The observed output closely matches the theoretical boost converter relationship:

Vout = Vin / (1 − D)

where D is the duty cycle.

## Applications

- Solar Power Systems
- Battery-Powered Devices
- Power Banks
- LED Drivers
- Electric Vehicles
- Embedded Systems
- Industrial Electronics

## Software Used

- LTspice XVII

## Author

Sujal Patil
