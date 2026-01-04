# Hamiltonian Origin and Numerical Verification of the Cross-Resonance ZX Interaction

This repository presents a Hamiltonian-level study of the cross-resonance (CR)
gate, focusing on the microscopic origin and numerical verification of the
effective conditional ZX interaction.

The goal of this work is to go beyond phenomenological gate models and provide a
clear derivation starting from a microscopic cavity-QED Hamiltonian, followed by
numerical validation of the resulting effective dynamics.

---

## Overview

We consider two two-level systems (qubits) dispersively coupled to a common
cavity resonator. Starting from a Jaynes–Cummings description, we eliminate the
cavity degrees of freedom using a Schrieffer–Wolff transformation, obtaining an
effective qubit–qubit exchange interaction of the form XX + YY.

By introducing a resonant drive on one qubit, moving to an appropriate rotating
frame, and performing a dressed-state transformation followed by a secular
approximation, we show that an effective conditional interaction emerges:

H_ZX = J_ZX σ_z1 σ_x2

This effective Hamiltonian is verified numerically through conditional Rabi
oscillations and Bell-state generation confirmed via von Neumann entropy.

---

## Repository Contents

### derivations/

Contains the full analytical derivation in PDF form, starting from the
microscopic Hamiltonian and leading to the effective ZX interaction.

### notebooks/

Contains Jupyter notebooks that numerically verify the effective Hamiltonian and
demonstrate conditional dynamics and entanglement generation.

---

## Frames and Scope

The analytical derivation makes extensive use of rotating frames, dressed-state
transformations, and interaction-picture arguments to isolate the slow dynamics
responsible for the CR gate.

The numerical simulations are performed in the interaction picture associated
with the dressed control-qubit Hamiltonian. Single-qubit control pulses are
treated as separate Hamiltonian terms when required.

Extension to full lab-frame simulations, pulse-level modeling, and noise effects
is left for future work.

---

## Status and Intent

This repository is intended as a physics-first, transparent account of how the
cross-resonance ZX interaction arises and how it can be identified and validated
numerically.

It is suitable as:
- a reference for Hamiltonian-level understanding of CR gates,
- a companion to theoretical studies of driven entangling interactions,
- a starting point for further extensions.

---

## Requirements

The numerical notebook relies on standard scientific Python tools, including:
- numpy
- qutip
- matplotlib

Exact versions are not pinned.

---

## License

This repository is provided for academic and educational use.
