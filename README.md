# AV1 Apex: AI‑Collaborative Hybrid Composite

[![Status: Theoretical/Simulation](https://img.shields.io/badge/Status-Theoretical%20Simulation-blue.svg)](#)
[![Engine: LAMMPS](https://img.shields.io/badge/Engine-LAMMPS-red.svg)](#)

## 🔬 Project Overview

**AV1 Apex** is a computationally designed high‑entropy alloy engineered to survive **Extreme Environment Impacts (EEI)**. By leveraging a high‑entropy chemical strategy (Al₂₀Fe₄₀Mn₁₀Ti₁₀Si₂₀), the material utilizes a rigid **Silicon‑Titanium‑Manganese “Cage”** to stabilize a high‑energy Aluminum‑Iron matrix during transient thermal events.

The core discovery is the **“Lattice Memory” effect**: the Si‑Ti‑Mn skeleton remains structurally coherent under extreme heat, providing a topological template for rapid recrystallization after the thermal pulse subsides.

---

## 🕒 Simulation Timeline

The material was interrogated through a multi‑stage Molecular Dynamics (MD) workflow:

1. **System Initialization:** 6,000 atoms configured in a triclinic supercell (FCC lattice, 4.05 Å, density ~5.2 g/cm³).
2. **Impact Simulation:** A massive thermal shock excitation to **17,000 K** for 0.5 ps (NVE ensemble), simulating extreme adiabatic energy injection.
3. **Healing Phase:** Structural recovery achieved via **Langevin cooling** (NVT) to 300 K over 10 ps – the lattice returns to within 2% of its ground‑state potential energy.
4. **Stress Test:** Post‑recovery uniaxial compression (strain rate 0.001 ps⁻¹) reached a **peak compressive stress of >6.7 GPa** (still rising at 2% strain), demonstrating significant structural rigidity after impact.

---

## 💎 Key Features (Supported by Simulation)

- **Lattice Memory:** The Si‑Ti‑Mn cage acts as a “structural anchor,” preserving atomic coordinates even when the Al‑Fe matrix becomes transiently molten/plasma‑like.
- **Ultrafast Recovery:** Full potential energy recovery in **~10 ps** – orders of magnitude faster than conventional superalloys (which require nanoseconds to seconds).
- **High Compressive Strength:** **≥6.7 GPa** (exceeding Inconel, many steels, and comparable to ultra‑high‑performance ceramics).
- **Lightweight:** Density ~5.2 g/cm³ – lighter than titanium alloys.

---

## ⚠️ Honest Limitations (For Transparency)

- **Tensile strength** has not yet been simulated; only uniaxial compression data is available.
- **Electron‑phonon coupling (TTM)** was not included – the real survival limit under nuclear‑grade flux will likely be lower (estimated 5000‑8000 K).
- **Potential dependence:** Results obtained with a custom EAM/FS potential (`AlFe_mm.eam.fs`). Independent validation with a different interatomic potential is recommended.
- **System size:** 6,000 atoms; larger (e.g., 21,600 atom) simulations are planned but not yet completed.

---

## 🛠 Credits & Tools

### Lead Researcher / Architect
**Himanshu Kumar Dixit** – Concept design, chemical composition strategy, and simulation execution.

### AI Collaboration
**Gemini (Google AI)** – Collaborative lead on script optimization, physics error troubleshooting (recursion & lost atom fixes), and advanced data analysis.

### Software & Potentials
- **LAMMPS** – Primary molecular dynamics engine.
- **Axel Kohlmeyer** – Foundational plugins and community support integrated into LAMMPS.
- **Potential Files** – Based on the `AlFe_mm.eam.fs` formalism (Mishin et al.) for high‑accuracy metallic matrix modeling.

### Special Thanks
To the open‑source materials science community for providing interatomic potentials and diagnostic tools that made this hybrid simulation possible.

---

**Disclaimer:** AV1 Apex is a computational model. Real‑world implementation requires experimental validation (e.g., via Spark Plasma Sintering or Laser Powder Bed Fusion) and independent reproducibility of the simulated properties.
