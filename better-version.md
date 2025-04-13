# 📚 Math & Microelectronics Daily Study Plan  
*(Total Duration: ~24-30 months | 5 days/week)*  

---

## Semester 1: Foundations (Weeks 1-20)  
**Goal:** Build a 2.4GHz PA while mastering algebra, calculus, and circuit analysis.  

### Week 1: DC Circuits & Algebra  
**Objective:** Calculate voltages/currents in simple circuits.  

| Day | Topic                      | What to Learn                          | Why Learn It?                                                                 | Activity                                                                 | Tools               |
|-----|----------------------------|----------------------------------------|-------------------------------------------------------------------------------|--------------------------------------------------------------------------|---------------------|
| 1   | Ohm's Law                  | Relationship between V, I, R           | Foundation for analyzing **all electronic circuits**                          | Simulate V=IR in LTSpice; solve for missing variable                     | Multimeter, LTSpice |
| 2   | Series/Parallel Resistors  | Equivalent resistance calculations     | Critical for designing voltage dividers and current-limiting circuits         | Build a 2-resistor circuit; measure total resistance                     | Breadboard, resistors |
| 3   | Kirchhoff's Laws           | Conservation of energy/charge in loops | Enables analysis of complex circuits (e.g., multi-branch networks)            | Solve for currents in a 3-resistor loop using algebraic systems          | Python (SymPy)      |
| 4   | Voltage Dividers           | Output voltage calculation (Vout = Vin*(R2/(R1+R2))) | Used in biasing transistors and sensor interfacing               | Design a divider to convert 9V → 3.3V; validate with multimeter          | Potentiometer       |
| 5   | Power Dissipation          | P = IV, derating components            | Prevents overheating/burning components in your PA design                     | Calculate max current for a 1/4W resistor; test with LED circuit         | Thermal camera      |

---

### Week 2: AC Circuits & Functions  
**Objective:** Analyze frequency-dependent behavior in circuits.  

| Day | Topic                      | What to Learn                          | Why Learn It?                                                                 | Activity                                                                 | Tools               |
|-----|----------------------------|----------------------------------------|-------------------------------------------------------------------------------|--------------------------------------------------------------------------|---------------------|
| 1   | Capacitors/Inductors       | Reactance (X_C = 1/(2πfC), X_L = 2πfL) | Key for filtering noise in RF circuits (e.g., PA input matching)              | Measure capacitor charge/discharge curve with oscilloscope              | Oscilloscope, 555 timer |
| 2   | RC Time Constant           | τ = RC, transient response            | Impacts signal rise/fall times in digital control for your PA                 | Plot charging curve vs. theory using Python                             | Python (Matplotlib) |
| 3   | AC Signals & Sinusoids     | Frequency, amplitude, phase           | All RF signals (e.g., 2.4GHz PA input) are sinusoidal                         | Generate 1kHz sine wave; measure Vpp                                    | Signal generator    |
| 4   | Function Transformations   | Shifts, stretches, compositions        | Needed to model modulated signals (e.g., AM/FM in SDR projects)               | Code a function in Python to shift/stretch a sine wave                  | Jupyter Notebook    |
| 5   | Filters (LPF/HPF)          | Cutoff frequency (f_c = 1/(2πRC))      | Remove unwanted frequencies (e.g., harmonics in PA output)                    | Design a 1kHz LPF; test attenuation at 10kHz                            | NanoVNA            |

---

## Semester 2: Digital Systems & Linear Algebra (Weeks 21-36)  
**Goal:** Control PAs digitally via USB using matrix operations.  

### Week 11: Digital Logic & Vectors  
**Objective:** Interface STM32 with logic gates.  

| Day | Topic                      | What to Learn                          | Why Learn It?                                                                 | Activity                                                                 | Tools               |
|-----|----------------------------|----------------------------------------|-------------------------------------------------------------------------------|--------------------------------------------------------------------------|---------------------|
| 1   | Boolean Algebra            | AND/OR/NOT gates, truth tables         | Basis for programming STM32 GPIO to control PA enable/disable                 | Build a NAND gate circuit; validate with logic analyzer                  | 74HC00 IC, logic analyzer |
| 2   | Vectors                    | Magnitude, direction, operations       | Used in beamforming (phased arrays) and sensor data representation            | Code vector addition in Python; plot results                            | NumPy              |
| 3   | Voltage Level Shifting     | 3.3V ↔ 5V interfacing                  | STM32 (3.3V) must safely control 5V components (e.g., PA bias circuits)        | Design a level shifter with MOSFET; test with oscilloscope               | 2N7000 MOSFET      |
| 4   | Matrices                   | Multiplication, transpose              | Core for MIMO processing in 5G/6G systems                                     | Solve a resistor network using matrix algebra                           | MATLAB/Octave      |
| 5   | Finite State Machines      | Transitions, outputs                   | Model USB protocol states (e.g., enumeration, data transfer)                  | Code a vending machine FSM in Python                                    | STM32CubeIDE       |

---

*(Continue pattern for subsequent weeks, integrating math topics with practical PA/SDR projects.)*
