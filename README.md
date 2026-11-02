# Type-I Phase-Locked Loop (PLL) Simulation Using LTspice

## 📌 Project Overview

This project demonstrates the design and transient simulation of a **Type-I Phase-Locked Loop (PLL)** using LTspice.

The PLL consists of a phase detector, an RC loop filter, and a voltage-controlled oscillator (VCO). The objective is to investigate the PLL's locking behavior, control-voltage convergence, and synchronization between the input and output signals.

Transient analysis and FFT analysis are performed to examine the circuit's behavior and verify frequency locking.

## ⚙️ Circuit Specifications

| Component / Parameter | Value |
|---|---:|
| PLL Architecture | Type-I PLL |
| Phase Detector | XOR-based |
| Loop Filter Resistor | 200 Ω |
| Loop Filter Capacitor | 50 nF |
| Input Signal | Sinusoidal |
| Input Frequency | 1 MHz |
| VCO Lower Frequency | 0.5 MHz |
| VCO Upper Frequency | 1.5 MHz |
| Initial VCO Control Voltage | 0.2 V |
| Transient Simulation Time | 350 µs |
| Simulation Tool | LTspice |

## 🔌 Circuit Architecture

The PLL consists of three main functional blocks connected in a feedback configuration:

1. **Phase Detector:** Compares the phase of the reference input signal with the feedback signal from the VCO. An XOR-based phase detector generates an error signal based on the phase difference.
2. **RC Loop Filter:** Filters the phase detector output to generate a smoother control voltage for the VCO.
3. **Voltage-Controlled Oscillator (VCO):** Generates an output signal whose frequency varies according to the control voltage. The output is fed back to the phase detector to complete the feedback loop.

## 🖥️ Simulation Configuration

The circuit was simulated in LTspice using transient analysis.

### Simulation Parameters

| Parameter | Value |
|---|---:|
| Analysis Type | Transient |
| Simulation Duration | 350 µs |
| Input Frequency | 1 MHz |
| VCO Frequency Range | 0.5–1.5 MHz |
| Loop Filter Resistance | 200 Ω |
| Loop Filter Capacitance | 50 nF |

## 📊 Simulation Results

### 1. FFT Analysis of VCO Output

The FFT of the VCO output was examined to observe its frequency-domain characteristics and identify the dominant frequency component.

### 2. Control Voltage Response

The control voltage initially exhibits transient oscillations before approaching a steady-state value around 0.49 V. This behavior illustrates the convergence of the PLL feedback loop.

### 3. Input and Output Signal Comparison

The reference input signal (Vin) and VCO output signal (Vout) were compared through transient waveform analysis.

The waveforms demonstrate the synchronization behavior of the PLL as the VCO adjusts its output frequency in response to the phase detector and loop filter.

### 4. PLL Lock Verification

The PLL locking behavior was examined by observing the control voltage and comparing the input and output waveforms.

The steady-state control voltage and synchronized waveform behavior provide evidence of the PLL approaching its locked condition.

## 🛠️ Tools and Technologies

- LTspice
- Transient Analysis
- FFT Analysis
- Phase Detector
- RC Loop Filter
- Voltage-Controlled Oscillator (VCO)
- PLL Feedback System

## 📚 Key Learning Outcomes

- Understanding the operating principle of a Type-I PLL.
- Implementing an XOR-based phase detector.
- Designing an RC loop filter.
- Understanding the relationship between control voltage and VCO frequency.
- Analyzing transient response and control-voltage convergence.
- Performing FFT analysis to investigate frequency-domain behavior.
- Evaluating PLL frequency locking through waveform comparison.

## 👨‍💻 Author

**Sheikh Tariful Islam**

Electrical and Electronic Engineering

Bangladesh University of Engineering and Technology (BUET)
