# 📚 Math & Electronics Roadmap for RF Engineering  
**Target**: Master foundational math and apply it to circuits, RF, and wireless systems.  

---

## 🧮 **Lesson 1: Algebra, Trigonometry, Functions (4-6 Weeks)**  
**Goal**: Relearn high school math and apply to basic circuits.  

### 1. **Algebra Basics**  
- **Topics**:  
  - Solving linear equations (e.g., Ohm’s Law: \( V = IR \)).  
  - Systems of equations (Kirchhoff’s Laws).  
  - Polynomials and factoring.  
- **Books**:  
  - *Algebra I for Dummies* – Mary Jane Sterling.  
  - *Practical Electronics for Inventors* (Ch. 1) – Applied examples.  
- **Courses**:  
  - [Khan Academy: Algebra Basics](https://www.khanacademy.org/math/algebra)  
- **Project**:  
  - Calculate resistor values for a voltage divider: \( V_{out} = V_{in} \cdot \frac{R_2}{R_1 + R_2} \).  

### 2. **Functions and Graphs**  
- **Topics**:  
  - Linear, quadratic, and exponential functions.  
  - Plotting voltage vs. current.  
- **Books**:  
  - *Precalculus: Mathematics for Calculus* – Stewart, Redlin (Ch. 1-2).  
- **Project**:  
  - Graph capacitor charging: \( V(t) = V_0(1 - e^{-t/RC}) \).  

### 3. **Trigonometry**  
- **Topics**:  
  - Sine, cosine, tangent (AC waveforms).  
  - Phasor diagrams.  
- **Books**:  
  - *Trigonometry for Dummies* – Mary Jane Sterling.  
- **Courses**:  
  - [Khan Academy: Trigonometry](https://www.khanacademy.org/math/trigonometry)  
- **Project**:  
  - Analyze AC circuit: \( V(t) = V_p \sin(2\pi ft) \).  

---

## 📈 **Lesson 2: Calculus, Complex Numbers, Differential Equations (6-8 Weeks)**  
**Goal**: Master calculus and complex numbers for RF design.  

### 1. **Calculus Basics**  
- **Topics**:  
  - Limits (capacitor charging).  
  - Derivatives (\( \frac{dV}{dt} \) in RC circuits).  
  - Integrals (energy in inductors).  
- **Books**:  
  - *Calculus for Dummies* – Mark Ryan.  
- **Courses**:  
  - [MIT OpenCourseWare: Single Variable Calculus](https://ocw.mit.edu/courses/18-01sc-single-variable-calculus-fall-2010/)  
- **Project**:  
  - Simulate derivative of a square wave (LTSpice).  

### 2. **Complex Numbers**  
- **Topics**:  
  - Rectangular/polar forms (\( a + jb \)).  
  - Euler’s formula (\( e^{j\theta} = \cos\theta + j\sin\theta \)).  
- **Books**:  
  - *Advanced Algebra* – Gelfand (Ch. 6).  
- **Courses**:  
  - [3Blue1Brown: Complex Numbers](https://www.youtube.com/watch?v=5PcpBw5Hbwo)  
- **Project**:  
  - Design LC filter: \( Z = j\omega L + \frac{1}{j\omega C} \).  

### 3. **Differential Equations**  
- **Topics**:  
  - First-order (RC/RL: \( \frac{dV}{dt} + \frac{V}{RC} = 0 \)).  
  - Second-order (RLC: \( LC\frac{d^2V}{dt^2} + RC\frac{dV}{dt} + V = 0 \)).  
- **Books**:  
  - *Differential Equations for Dummies* – Steven Holzner.  
- **Project**:  
  - Simulate RLC transient response (LTSpice).  

### 4. **Linear Algebra (Preview)**  
- **Topics**:  
  - Vectors/matrices (MIMO in 5G).  
- **Books**:  
  - *Linear Algebra Done Right* – Sheldon Axler.  
- **Project**:  
  - Solve resistor network with matrices.  

---

## 🛠️ **Tools & Resources**  
| **Tool**          | **Budget Option**                     | **Use Case**                |  
|--------------------|---------------------------------------|-----------------------------|  
| **Calculator**     | Casio fx-991EX ($20)                  | Complex numbers, matrices.  |  
| **Simulation**     | [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) (Free) | Circuit analysis. |  
| **Graphing**       | [Desmos](https://www.desmos.com/) (Free) | Plot functions.        |  

---

## 📌 **Weekly Schedule Example**  
| **Week** | **Focus**                     | **Tasks**                                  |  
|----------|-------------------------------|--------------------------------------------|  
| 1-2      | Algebra & Ohm’s Law           | Complete Khan Academy modules + voltage divider project. |  
| 3-4      | Trigonometry & AC Circuits    | Plot sine waves, analyze RC charging.      |  
| 5-6      | Calculus Basics               | Simulate derivatives in LTSpice.           |  
| 7-8      | Complex Numbers               | Design LC filter, validate with NanoVNA.   |  

---

## 🎯 **Validation Checklist**  
- [ ] Solve \( V = IR \) for unknown resistor values.  
- [ ] Graph \( V(t) \) for an RC circuit.  
- [ ] Simulate RLC transient response.  
- [ ] Design 50Ω microstrip line (KiCad).  

**Next Step**: Proceed to **Lesson 3 (Probability & Statistics)** for noise analysis in wireless systems!  
