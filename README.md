# AV1 Apex: AI-Collaborative Hybrid Composite

## 🔬 Project Overview
**AV1 Apex** is a pioneering theoretical hybrid composite engineered to survive **Extreme Environment Impacts (EEI)**. By leveraging a high-entropy chemical strategy, the material utilizes a rigid **Silicon-Titanium "Cage"** to stabilize a high-energy **Molten Aluminum-Iron matrix** during transient thermal events.

The core discovery is the **"Lattice Memory" effect**, where the Si-Ti skeleton remains structurally coherent under extreme heat, providing a topological template for near-instantaneous recrystallization.

---

## 🕒 Simulation Timeline
The material was interrogated through a multi-stage Molecular Dynamics (MD) workflow:

1.  **System Initialization:** 21,600 atoms configured in a high-fidelity triclinic supercell.
2.  **Impact Simulation:** A massive thermal shock excitation at **17,000 K**, simulating extreme adiabatic energy injection.
3.  **Healing Phase:** Rapid structural recovery achieved via stabilized **Langevin cooling** combined with **NPT Quenching** to restore lattice symmetry.
4.  **Stress Test:** Post-recovery mechanical validation reached a **Peak Tensile Stress of 14.46 GPa**, demonstrating significant structural hardening post-impact.

---

## 💎 Key Features
* **Lattice Memory:** The Si-Ti skeleton acts as a "structural anchor," converting impact energy into localized hardening rather than permanent failure.
* **Ultrafast Recovery:** Structural resetting occurs on a picosecond timescale, making it ideal for repetitive high-energy environments.
* **High Specific Strength:** Exhibits a strength-to-weight ratio an order of magnitude higher than conventional aerospace-grade titanium or steel.

---

## 🛠 Credits & Tools

### **Lead Researcher / Architect**
* **Himanshu Kumar Dixit** – Concept design, chemical composition strategy, and simulation execution.

### **AI Collaboration**
* **Gemini (Google AI)** – Collaborative lead on script optimization, physics error troubleshooting (recursion & Lost Atom fixes), and advanced data analysis.

### **Software & Potentials**
* **LAMMPS (Large-scale Atomic/Molecular Massively Parallel Simulator):** Primary molecular dynamics engine.
* **Axel Kohlmeyer:** For the foundational plugins and community support integrated into the LAMMPS environment.
* **Potential Files:** Based on the `AlFe_mm.eam.fs` formalism (Mishin et al.) for high-accuracy metallic matrix modeling.

### **Special Thanks**
* To the open-source materials science community for providing the interatomic potentials and diagnostic tools that made this hybrid simulation possible.

---

---
*Disclaimer: AV1 Apex is a computational model. Real-world implementation requires validation via Spark Plasma Sintering (SPS) or Laser Powder Bed Fusion (LPBF).*
