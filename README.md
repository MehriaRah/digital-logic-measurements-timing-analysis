# digital-logic-measurements-timing-analysis
A comprehensive analysis of 7400-series NAND gate characteristics, focusing on static logic verification, timing analysis (rise/fall times, propagation delay), and glitch observation using an oscilloscope and function generator


## Overview
[cite_start]This project documents a series of laboratory experiments conducted to measure the physical and timing characteristics of Small-Scale Integration (SSI) Integrated Circuits (ICs)[cite: 47, 52]. [cite_start]Specifically, it evaluates the **7400-series NAND gate** to understand the practical deviations from ideal Boolean logic, such as propagation delay and signal glitches[cite: 62, 343, 306].

## Objectives
* [cite_start]Setup and calibrate signal generation and measurement equipment (Oscilloscope, Function Generator, Power Supply)[cite: 49, 119].
* [cite_start]Characterize static logic behavior and verify truth tables[cite: 52, 148].
* [cite_start]Measure high-speed timing parameters including rise/fall times and propagation delay ($t_{pd}$)[cite: 150, 340].
* [cite_start]Observe and analyze combinatorial glitches caused by unequal path delays[cite: 306, 307].

## Hardware & Tools Used
* [cite_start]**IC:** 7400 Quad 2-input NAND Gate[cite: 62].
* [cite_start]**Equipment:** Function Generator, Digital Oscilloscope (RTB2004), IC Evaluation Board[cite: 119, 287].
* [cite_start]**Power Supply:** $V_{cc} = 3.3V$[cite: 328].

## Lab Tasks & Results

### 1. Static Behavior Verification
[cite_start]The logic functionality was tested using manual switches and LED indicators[cite: 329].
* [cite_start]**Observation:** The gate successfully matched the NAND truth table (Output '0' only when both inputs are '1') [cite: 332-335].

### 2. Timing Characteristics
[cite_start]Using a square wave (10-100 kHz) as a stimulus, the following timing parameters were captured at the 10%/50%/90% voltage thresholds[cite: 339, 356, 375]:

| Parameter | Measured Value | Definition |
| :--- | :--- | :--- |
| **Input Rise Time ($t_r$)** | 2.5 ns | [cite_start]10% to 90% of full swing [cite: 363, 357] |
| **Output Fall Time ($t_f$)** | 3.5 ns | [cite_start]90% to 10% of full swing [cite: 373, 366] |
| **Propagation Delay ($t_{pd}$)** | 5.0 ns - 8.3 ns | [cite_start]50% input crossing to 50% output crossing [cite: 381, 295] |


### 3. Glitch Observation
[cite_start]The lab explored "glitches"—brief, unwanted pulses occurring during input transitions[cite: 306].
* **Analysis:** These are caused by unequal propagation delays across different internal paths[cite: 307].
* [cite_start]**Result:** Observed short pulses (nanosecond scale) during switching, highlighting the importance of timing synchronization in complex combinatorial logic[cite: 308, 313].

## Key Technical Skills Demonstrated
* [cite_start]**Oscilloscope Proficiency:** Utilizing 50% crossing methods and cursors for nanosecond-scale measurements[cite: 291, 299].
* **Signal Integrity:** Identifying overshoot (<10%) and ringing caused by parasitic capacitance/inductance in probes[cite: 383, 309].
* [cite_start]**Circuit Troubleshooting:** Configuring function generators with 50Ω termination to prevent signal reflections[cite: 127, 128].


<img width="1280" height="824" alt="2 2 task" src="https://github.com/user-attachments/assets/49ba113a-babf-4c93-a6fc-20dfce5d538f" />

<img width="1200" height="1600" alt="WhatsApp Image 2026-05-08 at 13 57 56" src="https://github.com/user-attachments/assets/d5653f39-fb70-46b2-8acd-ac6e956dba5b" />


