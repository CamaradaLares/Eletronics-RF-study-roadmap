# 🎓 Microelectronics & RF Engineering: 5-Semester Master Plan  
*(Total Duration: ~18-24 months | Adjustable Pace)*  

## Legend  
- 📖 Book Chapter  
- 🔧 Project  
- ✅ Validation Test  
- ⚙️ Tools Needed  

### Color Code:  
- **Blue** = Fundamental  
- **Green** = Digital/USB  
- **Purple** = RF  
- **Red** = 5G/6G Research  

---

## 📅 Semester 1: Electronics & RF Crash Course (Weeks 1-20)  
**Goal:** Build a 2.4GHz 300mW Power Amplifier (PA) while mastering fundamentals.  

### Weekly Breakdown  

| Week | Focus Area       | 📖 Book Chapters                                                                 | 🔧 Project                     | ✅ Validation                          | ⚙️ Tools               |
|------|------------------|---------------------------------------------------------------------------------|--------------------------------|----------------------------------------|------------------------|
| 1    | DC Circuits      | *Make: Electronics (Ch. 1-2), Art of Electronics (Ch. 1)*                       | LED + resistor circuit         | Measure current (I = V/R)              | Multimeter             |
| 2    | AC Circuits      | *Practical Electronics (Ch. 3), ARRL Handbook (Ch. 4)*                         | 555 timer oscillator           | Verify 1kHz square wave                | Oscilloscope           |
| 3    | Transistors      | *Art of Electronics (Ch. 2), RF Microelectronics (Ch. 3)*                       | Class-A amp (2N3904)           | Gain ≥ 10dB (1kHz)                     | Signal generator       |
| 4    | LC Tanks         | *RF Circuit Design (Bowick, Ch. 2), ARRL Handbook (Ch. 6)*                     | 10MHz crystal oscillator       | Resonance within ±100ppm               | NanoVNA               |
| 5    | PCB Design       | *Getting Started with KiCad, PCB Currents (Ch. 3)*                              | 50Ω microstrip line            | S11 < -10dB @ 100MHz                   | KiCad, FR4 PCB        |
| 6    | LNAs             | *RF Microelectronics (Ch. 5), Experimental Methods (Ch. 4)*                     | 2.4GHz LNA (BFU730F)           | Gain ≥ 15dB, NF < 3dB                  | TinySA                |
| 7-8  | PAs              | *RF Power Amplifiers (Cripps, Ch. 3), ARRL Handbook (Ch. 14)*                  | 100MHz PA (2N5109)             | Output ≥ 100mW, η > 30%                | RF power meter        |
| 9-10 | Integration      | –                                                                               | 2.4GHz PA (MRF24G300HS)        | 300mW @ 2.4GHz, S11 < -15dB            | Spectrum analyzer     |

**Semester 1 Final Exam:**  
✅ Defend your PA design (Explain stability, efficiency, and matching).  

---

## 📅 Semester 2: Digital Systems & USB (Weeks 21-36)  
**Goal:** Master STM32, USB 2.0, and mixed-signal systems.  

### Key Projects  

| Week | Focus Area      | 📖 Book Chapters                                      | 🔧 Project                  | ✅ Validation                          | ⚙️ Tools               |
|------|-----------------|------------------------------------------------------|----------------------------|----------------------------------------|------------------------|
| 11   | Digital Logic   | *Digital Design (Harris, Ch. 1-3)*                  | 74HC00 logic tester        | Truth table matches                    | Logic analyzer        |
| 12   | STM32 Basics    | *Mastering STM32 (Ch. 1-3), Embedded Systems (Yiu)* | Blinky LED (HAL)           | GPIO toggles at 1Hz                    | STM32F4 Discovery     |
| 13   | USB-CDC         | *USB Complete (Ch. 3), STM32 USB OTG Guide*         | Virtual COM port           | "Hello World" over USB                 | USB protocol analyzer |
| 14   | USB HID         | *USB in a Nutshell (Beyond Logic)*                  | Custom USB keyboard        | Keypress registers                     | Wireshark (USB capture) |
| 15-16| RF Control      | –                                                   | STM32 + PA Control         | Adjust PA bias via USB                 | Custom PCB            |

**Semester 2 Final Exam:**  
✅ Stream sensor data to PC at 1Mbps over USB.  

---

## 📅 Semester 3: Advanced RF & Signal Integrity (Weeks 37-52)  
**Goal:** Phased arrays, RFICs, and EMI mitigation.  

### Key Projects  

| Week | Focus Area        | 📖 Book Chapters                            | 🔧 Project               | ✅ Validation                     | ⚙️ Tools               |
|------|-------------------|--------------------------------------------|--------------------------|-----------------------------------|------------------------|
| 17   | S-Parameters      | *Microwave Engineering (Pozar, Ch. 4)*    | 2.4GHz filter            | S21 > -3dB in band               | NanoVNA               |
| 18   | PCB Stackup       | *Signal Integrity (Bogatin, Ch. 7)*       | 4-layer FPGA board       | TDR shows Z0 = 50Ω ±10%          | Altium/KiCad          |
| 19-20| Phased Arrays     | *Phased Array Antennas (Hansen)*          | 2x2 patch array          | Beam steering ±30°               | ADAR1000 eval board   |

**Semester 3 Final Exam:**  
✅ Demo a beamforming array at 2.4GHz.  

---

## 📅 Semester 4: Capstone – 2.4GHz SDR + PA (Weeks 53-68)  
**Goal:** Build a software-defined radio with integrated PA.  

### Project Milestones  
- **SDR Frontend** (LimeSDR/RTL-SDR + 2.4GHz PA).  
- **STM32 Baseband Processor** (USB 2.0 HS).  
- **GNU Radio Companion** (FSK modulation/demod).  
- **FCC Pre-Compliance Test** (Scan for spurs).  

**Validation:**  
✅ Transmit/receive WiFi beacon packets.  

---

## 📅 Semester 5: 5G/6G Research (Weeks 69-84)  
**Goal:** mmWave, massive MIMO, and RFIC design.  

### Key Projects  

| Week | Focus Area   | 📖 Book Chapters               | 🔧 Project            | ✅ Validation            | ⚙️ Tools               |
|------|--------------|--------------------------------|-----------------------|--------------------------|------------------------|
| 21   | 5G NR        | *5G NR (Dahlman, Ch. 6)*      | OFDM sim (Python)     | EVM < -25dB             | MATLAB/Python         |
| 22   | mmWave       | *mmWave Wireless (Rappaport, Ch. 3)* | 28GHz antenna | Beamwidth ≤ 10°         | HFSS                  |
| 23-24| RFIC         | *RFIC Design (Lee, Ch. 5)*    | LNA (Cadence)         | NF < 2dB @ 28GHz        | Cadence Virtuoso      |

**Semester 5 Final Exam:**  
✅ Publish findings on arXiv or present at IEEE conference.  

---

## 📚 Ultimate Book List  

### Core Texts  
- **Fundamentals:** *Art of Electronics (Horowitz), RF Microelectronics (Razavi)*.  
- **Digital/USB:** *Digital Design (Harris), USB Complete (Axelson)*.  
- **RF/5G:** *Microwave Engineering (Pozar), 5G NR (Dahlman)*.  
- **Tools:** *PCB Currents (Brooks), Signal Integrity (Bogatin)*.  

### Supplemental  
- *ARRL Handbook (for hands-on RF)*.  
- *GNU Radio for SDR (Blossom)*.  
- *RFIC Design (Lee)*.  

---

## 🛠️ Lab Equipment Checklist  

| Tool               | Budget Option         | Purpose                          |
|--------------------|-----------------------|----------------------------------|
| Oscilloscope       | Rigol DS1054Z ($250)  | Debug analog/digital.            |
| NanoVNA            | NanoVNA-H4 ($50)      | S11/S21 up to 3GHz.              |
| Spectrum Analyzer  | TinySA Ultra ($200)   | 6GHz RF analysis.                |
| RF Power Meter     | AD8307-based ($50)    | Measure PA output.               |
| 5G/mmWave         | ADI ADRV9009 ($1k)    | 6GHz SDR prototyping.            |

---

## 🎯 Graduation Requirements  

### Build & Test  
- 2.4GHz PA (300mW).  
- USB-controlled SDR.  
- 28GHz phased array prototype.  

### Publish Work  
- GitHub repo with full documentation.  
- White paper or conference submission.  

### Defend Knowledge  
- Explain Smith charts, OFDM, and RFIC design.  

---

## 📌 Weekly Time Commitment  
- **Theory:** 5-7 hours/week (books, papers).  
- **Lab Work:** 10+ hours/week (projects).  
- **Weekends:** Debugging/validation.  
