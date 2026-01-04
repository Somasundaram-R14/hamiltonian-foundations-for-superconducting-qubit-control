# Hamiltonian Origin and Numerical Verification of the Cross-Resonance ZX Interaction

This repository presents a Hamiltonian-level study of the cross-resonance (CR)
gate, focusing on the microscopic origin and numerical verification of the
effective conditional ZX interaction.

This work represents one component of a broader program aimed at understanding
entangling gates and noise processes directly from microscopic Hamiltonians,
rather than phenomenological gate models.

---

## Overview

We consider two two-level systems (qubits) dispersively coupled to a common
cavity resonator. Starting from a Jaynes–Cummings description, we eliminate the
cavity degrees of freedom using a Schrieffer–Wolff transformation, obtaining an
effective qubit–qubit exchange interaction of the form XX + YY.

By introducing a resonant drive on one qubit, moving to an appropriate rotating
frame, and performing a dressed-state transformation followed by a secular
approximation, we show that an effective conditional interaction emerges:

$H_ZX = J_ZX σ_z1 σ_x2$

This effective Hamiltonian is verified numerically through conditional Rabi
oscillations and Bell-state generation confirmed via von Neumann entropy.

---

## Repository Contents

### derivations/

Contains analytical derivations in PDF form, starting from the microscopic
Hamiltonian and leading to effective interactions relevant for the
cross-resonance gate.

### notebooks/

Contains Jupyter notebooks providing numerical verification and physical
interpretation of the effective Hamiltonians derived in this work.

---

## Frames, Approximations, and Scope

The analytical derivations make extensive use of rotating frames,
dressed-state transformations, and interaction-picture arguments in order to
isolate the slow dynamics responsible for conditional entangling interactions.

The numerical simulations included here are performed in effective interaction
pictures appropriate for identifying the emergent ZX coupling. Single-qubit
control pulses are treated as separate Hamiltonian terms when required.

At this stage, the focus is on coherent Hamiltonian dynamics. Dissipative and
dephasing effects are not yet included.

---

## Relation to Future Work

This repository addresses the coherent Hamiltonian origin of the cross-resonance
ZX interaction. It is intended to serve as a foundation for future extensions,
including:

- Hamiltonian-level modeling of noise sources (e.g., dephasing and relaxation),
- dressing and renormalization of noise operators under dispersive and driven
  transformations,
- sensitivity of effective gate terms to microscopic noise processes,
- echoed and optimized CR gate constructions.

These extensions will be added incrementally as part of a larger effort to
connect microscopic Hamiltonians, effective gates, and noise-aware design.

---

## Status and Intent

This repository is intended as a physics-first, transparent account of how the
cross-resonance ZX interaction emerges from a driven dispersive system and how it
can be identified and validated numerically.

It is suitable as:
- a reference for Hamiltonian-level understanding of CR gates,
- a foundation for noise-aware gate analysis,
- a starting point for further theoretical and numerical extensions.

---

## Requirements

The numerical notebooks rely on standard scientific Python tools, including:
- numpy
- qutip
- matplotlib

Exact versions are not pinned at this stage.

---

## License

This repository is provided for academic and educational use.
