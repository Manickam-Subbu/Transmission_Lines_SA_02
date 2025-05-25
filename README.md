# 🚀 Design and Simulation of a High-Frequency Rectangular Waveguide for ISRO Communication Satellites

![Waveguide Banner](images/waveguide_diagram.png)

## 📚 Table of Contents
- [Project Overview](#project-overview)
- [Objective](#objective)
- [Background](#background)
- [Specifications](#specifications)
- [Design Methodology](#design-methodology)
- [Simulation Tools](#simulation-tools)
- [Results](#results)
- [Applications](#applications)
- [Contributing](#contributing)
- [License](#license)

---

## 🛰️ Project Overview

This project involves the **design, simulation, and analysis of a high-frequency rectangular waveguide** intended for **Ka-band (26.5 – 40 GHz)** satellite communication systems used by **ISRO**. It focuses on electromagnetic field distribution, cut-off frequencies, and S-parameter analysis.

---

## 🎯 Objective

- Design a standard WR-28 waveguide (Ka-band).
- Simulate TE modes and identify dominant mode propagation.
- Analyze field distribution and scattering parameters.
- Investigate application in ISRO satellite systems.

---

## 🔍 Background

A **rectangular waveguide** is a type of transmission line used in microwave systems. For satellite communication, waveguides offer **low loss**, **high power handling**, and **mode selectivity**.

### 📐 Basic TE10 Mode Field Equation:

\[
f_c = \frac{c}{2a}, \quad \text{where } a \text{ is the wider dimension}
\]

For WR-28:

| Parameter     | Value         |
|---------------|---------------|
| `a` (Width)   | 7.112 mm      |
| `b` (Height)  | 3.556 mm      |
| Frequency     | 26.5–40 GHz   |
| Dominant Mode | TE₁₀          |

---

## ⚙️ Design Methodology

### 📌 Steps Followed:
1. **Geometry Modeling** (WR-28 dimensions)
2. **Material Assignment** (Perfect conductor walls, air-filled)
3. **Boundary Conditions**: PEC (Perfect Electric Conductor)
4. **Excitation**: Port excitation for TE₁₀ mode
5. **Simulation**: Frequency sweep (26.5 – 40 GHz)
6. **Post Processing**: S-parameters, field plots

### 📊 Diagram: Field Configuration

![TE10 Field Distribution](images/field_pattern.png)

---

## 🛠️ Simulation Tools

| Tool           | Purpose                      |
|----------------|------------------------------|
| ANSYS HFSS     | 3D EM Simulation              |
| CST Studio     | Verification and optimization |
| MATLAB         | Cut-off frequency analysis    |
| Python         | Data analysis (S-parameters)  |

---

## 📈 Results

### ✔️ S-Parameter Plot:
- **S11**: Below -15 dB in operational band
- **S21**: Close to 0 dB (low loss transmission)

### ✔️ Field Pattern:
- TE₁₀ mode confirmed (maximum field in width)

| Frequency (GHz) | S11 (dB) | S21 (dB) |
|------------------|----------|----------|
| 28               | -18.5    | -0.8     |
| 30               | -22.1    | -0.3     |
| 35               | -19.9    | -0.5     |

---

## 🇮🇳 Applications in ISRO

- **GSAT Series Satellites**: C/Ku/Ka Band communication payloads.
- **GAGAN & NavIC Systems**: Precision navigation requiring low-loss waveguides.
- **Payload testing labs (ISTRAC/URSC)**: Internal waveguide designs.

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss your ideas.

---

## 📄 License

This project is open-source under the MIT License.

---

## 📎 References

- Pozar, D. M. *Microwave Engineering*, 4th Ed.
- ISRO Technical Docs – [https://www.isro.gov.in](https://www.isro.gov.in)
- ANSYS HFSS & CST Studio Suite Documentation

