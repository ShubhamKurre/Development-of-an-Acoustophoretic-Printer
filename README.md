# 🔊 Development of an Acoustophoretic Printer

This project focuses on the **design and development of an acoustophoretic droplet-printing system**, integrating a **subwavelength acoustic resonator** with a **CNC 3018 motion platform**.  
The printer enables **contactless, viscosity-agnostic droplet ejection** for applications in **bioprinting, functional inks, and lab-on-chip systems**.


---

## 🎯 Objectives
- Design a **subwavelength acoustic resonator** capable of generating focused acoustic radiation pressure for droplet ejection.
- Integrate the resonator with a **3-axis CNC platform** for controlled spatial positioning.
- Characterize droplet formation across **varied viscosities (1–500 mPa·s)** and correlate results with theoretical models.
- Demonstrate **non-contact, controllable droplet deposition** for multi-material printing.

---

## 🧠 Background

**Acoustophoretic printing** uses sound waves instead of mechanical nozzles to eject droplets.  
By generating a standing acoustic wave inside a resonator, localized pressure nodes form — capable of **propelling droplets** from a liquid meniscus without physical contact.  

This eliminates issues like **nozzle clogging**, **shear damage to biofluids**, and **material dependency**, making it ideal for:
- **Bioprinting (cell-laden gels, proteins)**
- **Functional inks and polymers**
- **Microfluidic and lab-on-chip patterning**

---

## 🧰 Tools & Components
| Component | Description |
|------------|-------------|
| **CNC 3018 platform** | Provides precise 3-axis motion control (±0.01 mm) |
| **Piezoelectric transducer (40 kHz)** | Generates standing acoustic field |
| **Signal generator + amplifier** | Controls amplitude and frequency |
| **Function controller (Arduino/CNC GRBL)** | Coordinates droplet positioning |
| **High-speed camera (1000 fps)** | Captures droplet ejection dynamics |
| **MATLAB / Python** | Data analysis and theoretical modeling |

---

## ⚙️ Methodology

### 1. Acoustic Resonator Design
- Designed **subwavelength cavity (λ/2)** geometry using COMSOL and analytical equations.  
- Optimized for **40 kHz resonance** to produce uniform standing wave pattern.  
- Verified **acoustic pressure distribution** via simulation.

### 2. Integration with CNC Platform
- Mounted transducer and liquid reservoir onto the CNC’s Z-axis carriage.
- Used **GRBL G-code control** for spatial droplet deposition.
- Achieved **stepwise motion of 0.1 mm** for accurate pattern formation.

### 3. Droplet Formation & Characterization
- Conducted droplet ejection experiments under quasi-static conditions.
- Recorded droplet size and velocity using high-speed imaging.
- Observed **80–120 μm droplet diameter**, consistent with theoretical predictions:
  
  \[
  F_{ac} = \frac{2 \pi P_0^2}{\rho c^2 \lambda}
  \]

### 4. Theoretical Validation
- Compared experimental droplet size with acoustic pressure-based ejection models.
- Validated performance for **viscosity range 1–500 mPa·s** (water to glycerol).

---

## 📊 Key Results

| Parameter | Value | Remarks |
|------------|--------|----------|
| Droplet Diameter | 80–120 μm | Matches theoretical λ/4 prediction |
| Frequency | 40 kHz | Subwavelength resonance |
| Viscosity Range | 1–500 mPa·s | Stable operation |
| Printing Mode | Contactless | No nozzle or mechanical actuation |
| Positioning Accuracy | ±0.01 mm | CNC-controlled stage |

---

## 🧪 Visuals

**Experimental Setup**  
![Setup Image](Results/acoustophoretic_setup.png)

**High-Speed Droplet Ejection Frames**  
![Droplet Frames](Results/droplet_frames.png)

**Pressure Field Simulation (COMSOL)**  
![Pressure Field](Results/pressure_field.png)

---

## 📚 Learning Outcomes
- Understood **acoustic wave–fluid interactions** and **radiation pressure theory**.
- Designed and fabricated an **acoustic resonator** for precision droplet generation.
- Integrated **hardware control (CNC + transducer)** with **signal electronics**.
- Applied **theoretical and experimental validation** for multi-viscosity liquids.
- Contributed toward a **contactless, biocompatible printing platform**.

---

## 🧭 Future Work
- Implement **closed-loop feedback** using computer vision for real-time droplet control.
- Extend to **multi-frequency actuation** for variable droplet size tuning.
- Explore **multi-material bioprinting** and **3D pattern generation**.

---

## 👨‍💻 Author
**Shubham Kurre**  
Mechanical Engineering | Acoustics | Fluid Mechanics | Mechatronics  
[LinkedIn](https://linkedin.com/in/) • [GitHub](https://github.com/shubhamkurre)

---

## 📂 Repository Structure
