# 📚 Microelectronics, RF, & Wireless Communications Study Plan  
**Prerequisite:** High school math. **Goal:** Master electronics, RF design, and 5G/6G systems.  

---

## 📅 Semester 1: Electronics & RF Crash Course (Weeks 1-20)  
**Goal:** Build a 2.4GHz PA while mastering fundamentals.  

### Weekly Breakdown  

| Week | Focus Area               | 📖 Books/Resources                                                                 | 🔧 Project                                                                 | ✅ Validation                                                                 |  
|------|--------------------------|-----------------------------------------------------------------------------------|----------------------------------------------------------------------------|------------------------------------------------------------------------------|  
| 1    | DC Circuits              | *Make: Electronics* (Ch. 1-2), *Art of Electronics* (Ch. 1)                       | LED + resistor circuit                                                    | Verify Ohm’s Law with multimeter                                             |  
| 2    | AC Circuits              | *Practical Electronics* (Ch. 3), *ARRL Handbook* (Ch. 4)                         | 555 timer oscillator                                                      | Measure 1kHz square wave (oscilloscope)                                      |  
| 3    | Transistors              | *Art of Electronics* (Ch. 2), *RF Microelectronics* (Razavi, Ch. 3)              | Class-A amplifier (2N3904)                                               | Measure gain ≥ 10dB (signal generator)                                       |  
| 4    | LC Tanks                 | *RF Circuit Design* (Bowick, Ch. 2), *ARRL Handbook* (Ch. 6)                     | 10MHz crystal oscillator                                                  | Verify resonance with NanoVNA (±100ppm)                                      |  
| 5    | PCB Design               | *Getting Started with KiCad*, *PCB Currents* (Brooks, Ch. 3)                     | 50Ω microstrip line                                                       | Measure S11 < -10dB @ 100MHz (NanoVNA)                                       |  
| 6    | LNAs                     | *RF Microelectronics* (Ch. 5), *Experimental Methods* (Hayward, Ch. 4)           | 2.4GHz LNA (BFU730F)                                                     | Gain ≥ 15dB, NF < 3dB (TinySA)                                               |  
| 7-8  | PAs                      | *RF Power Amplifiers* (Cripps, Ch. 3), *ARRL Handbook* (Ch. 14)                  | 100MHz PA (2N5109)                                                       | Output ≥ 100mW, efficiency > 30% (RF power meter)                             |  
| 9-10 | Integration              | –                                                                                | **2.4GHz PA (MRF24G300HS)**                                              | 300mW @ 2.4GHz, S11 < -15dB (spectrum analyzer)                              |  

**Final Project:**  
✅ Defend your PA design (explain stability, matching, and efficiency).  

---

## 📅 Semester 2: Digital Systems & USB (Weeks 21-36)  
**Goal:** Master STM32, USB 2.0, and mixed-signal systems.  

### Key Projects  

| Week | Focus Area         | 📖 Books/Resources                          | 🔧 Project                          | ✅ Validation                                  |  
|------|--------------------|--------------------------------------------|-------------------------------------|-----------------------------------------------|  
| 11   | Digital Logic      | *Digital Design* (Harris, Ch. 1-3)        | 74HC00 logic tester                | Truth table matches (logic analyzer)           |  
| 12   | STM32 Basics       | *Mastering STM32* (Noviello, Ch. 1-3)     | Blinky LED (HAL)                   | GPIO toggles at 1Hz                            |  
| 13   | USB-CDC            | *USB Complete* (Axelson, Ch. 3)           | Virtual COM port                   | "Hello World" over USB                         |  
| 14   | USB HID            | *USB in a Nutshell* (Beyond Logic)        | Custom USB keyboard                | Keypress registers (Wireshark)                 |  
| 15-16| RF Control         | –                                        | STM32 + PA Control                 | Adjust PA bias via USB                         |  

**Final Project:**  
✅ Stream sensor data to PC at 1Mbps over USB.  

---

## 📅 Semester 3: Advanced RF & Signal Integrity (Weeks 37-52)  
**Goal:** Phased arrays, RFICs, and EMI mitigation.  

### Key Projects  

| Week | Focus Area          | 📖 Books/Resources                          | 🔧 Project                          | ✅ Validation                                  |  
|------|---------------------|--------------------------------------------|-------------------------------------|-----------------------------------------------|  
| 17   | S-Parameters        | *Microwave Engineering* (Pozar, Ch. 4)    | 2.4GHz filter                      | S21 > -3dB in band (NanoVNA)                  |  
| 18   | PCB Stackup         | *Signal Integrity* (Bogatin, Ch. 7)       | 4-layer FPGA board                 | TDR shows Z0 = 50Ω ±10%                       |  
| 19-20| Phased Arrays       | *Phased Array Antennas* (Hansen)          | 2x2 patch array                    | Beam steering ±30° (ADAR1000 eval board)       |  

**Final Project:**  
✅ Demo a beamforming array at 2.4GHz.  

---

## 📅 Semester 4: Capstone – 2.4GHz SDR + PA (Weeks 53-68)  
**Goal:** Build a software-defined radio with integrated PA.  

### Milestones  
1. **SDR Frontend**: LimeSDR/RTL-SDR + 2.4GHz PA.  
2. **STM32 Baseband Processor**: USB 2.0 HS.  
3. **GNU Radio Companion**: FSK modulation/demod.  
4. **FCC Pre-Compliance Test**: Scan for spurs.  

**Validation:**  
✅ Transmit/receive WiFi beacon packets.  

---

## 📅 Semester 5: 5G/6G Research (Weeks 69-84)  
**Goal:** mmWave, massive MIMO, and RFIC design.  

### Key Projects  

| Week | Focus Area          | 📖 Books/Resources                          | 🔧 Project                          | ✅ Validation                                  |  
|------|---------------------|--------------------------------------------|-------------------------------------|-----------------------------------------------|  
| 21   | 5G NR               | *5G NR* (Dahlman, Ch. 6)                  | OFDM simulation (Python)           | Plot constellation diagram                    |  
| 22   | mmWave              | *mmWave Wireless* (Rappaport, Ch. 3)      | 28GHz patch antenna (HFSS)         | Simulate beamwidth ≤ 10°                      |  
| 23-24| RFIC Design         | *RFIC Design Fundamentals* (Lee, Ch. 5)   | LNA design (Cadence)               | Simulate NF < 2dB @ 28GHz                     |  

**Final Project:**  
✅ Publish findings on arXiv or present at IEEE conference.  

---

## 🔧 Tools & Resources  

### Electronics/RF Tools  
| **Tool**               | **Premium**              | **Budget Alternative**       |  
|-------------------------|--------------------------|------------------------------|  
| Oscilloscope            | Rigol DS1054Z ($400)     | Hantek 2C42 (USB, $150)      |  
| VNA                     | Keysight PNA ($10k+)     | NanoVNA-H4 ($50)             |  
| Spectrum Analyzer       | Siglent SSA3032X ($2k)   | TinySA Ultra ($200)          |  

### 5G/6G Tools  
| **Tool**               | **Premium**              | **Budget Alternative**       |  
|-------------------------|--------------------------|------------------------------|  
| SDR Transceiver         | USRP B210 ($1k)          | PlutoSDR ($200)              |  
| mmWave Dev Kit          | ADI ADRV9009 ($1.5k)     | MATLAB Simulations (Free)    |  

---

## 📚 Book List  

### Core Texts  
1. **Electronics**: *Art of Electronics* (Horowitz), *RF Microelectronics* (Razavi).  
2. **Digital/USB**: *Digital Design* (Harris), *USB Complete* (Axelson).  
3. **5G/6G**: *5G NR* (Dahlman), *mmWave Wireless* (Rappaport).  

### Math Fundamentals  
1. *Algebra I for Dummies* → *Calculus for Dummies* → *RF Microelectronics*.  
2. *Probability and Statistics for Engineering* (Devore).  

---

## 🎯 Graduation Checklist  
- ✅ Build a 2.4GHz PA (300mW).  
- ✅ Design a USB-controlled SDR.  
- ✅ Simulate 5G NR waveforms.  
- ✅ Publish research findings.  

**Next Steps:** Dive into RFIC design or 6G research!  
