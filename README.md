# 🔐 Quantum Key Distribution Simulator (BB84, B92, E91)

This project implements three fundamental **Quantum Key Distribution (QKD)** protocols — **BB84**, **B92**, and **E91** — to demonstrate secure key exchange and evaluate their robustness using **Quantum Bit Error Rate (QBER)** as a metric.

## 🚀 Features

- ✅ Simulation of BB84, B92, and E91 protocols  
- ✅ QBER computation under noise and real hardware conditions  
- ✅ Implemented using both **Qiskit** and **QuTiP** frameworks  
- ✅ Noise modeling via depolarizing channels  
- ✅ Supports Qiskit Local Simulator and IBM Quantum Hardware

## 📈 QBER Analysis

QBER is computed as:

```
QBER = (Number of mismatched bits) / (Number of matched basis rounds)
```

Results are collected and compared across:
- Qiskit Local Simulator
- IBM Quantum Hardware
- QuTiP (custom noise simulations)

## 🧠 Protocol Overview

- **BB84**: Uses random bases (Z/X) for encoding and decoding bits  
- **B92**: Utilizes two non-orthogonal states for simpler communication  
- **E91**: Based on entangled states and CHSH inequality for security verification

## 📂 Structure


├── ibm_B92.ipynb        # B92 on IBM Qiskit Hardware
├── ibm_BB84.ipynb       # BB84 on IBM Qiskit Hardware
├── ibm_E91.ipynb        # E91 on IBM Qiskit Hardware
├── qutip_B92.ipynb      # B92 using QuTiP
├── qutip_BB84.ipynb     # BB84 using QuTiP
├── qutip_E91.ipynb      # E91 using QuTiP
├── bb84_3.ipynb         # Extra BB84 testing notebook

## 📦 Requirements

- Python 3.8+
- Qiskit
- QuTiP
- NumPy
- Matplotlib (optional for plots)

Install with:
pip install qiskit qutip numpy matplotlib


---

Developed as a comparative study of QKD protocols under simulated and real quantum environments.
