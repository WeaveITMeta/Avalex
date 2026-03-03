# Quantum Chemistry Methods Overview

Table of Contents
- [Purpose](#purpose)
- [Method Categories](#method-categories)
  - [Ab Initio Wavefunction](#ab-initio-wavefunction)
  - [Post-HF Correlation (Single-Reference)](#post-hf-correlation-single-reference)
  - [Multi-Reference / Strongly Correlated](#multi-reference--strongly-correlated)
  - [Density Functional Theory (DFT)](#density-functional-theory-dft)
  - [Geometry Optimization & Vibrations](#geometry-optimization--vibrations)
  - [Intermolecular / Non-Covalent Interactions](#intermolecular--non-covalent-interactions)
  - [Excited States & Response Properties](#excited-states--response-properties)
  - [Relativistic & Core Treatments](#relativistic--core-treatments)
  - [Solvation & Environment](#solvation--environment)
  - [Properties & Analysis](#properties--analysis)

## Purpose
Organized reference for key quantum chemistry methods, principles, and example approaches for quick selection and study.

## Summary
- **Ab Initio Wavefunction** — Mean-field starting point; single-determinant HF orbitals. Use for cheap baselines and initial guesses.
- **Post-HF Correlation (Single-Reference)** — Add dynamic correlation (MP2–MP4, CCSD/CCSD(T)); high accuracy when a single reference is valid.
- **Multi-Reference / Strongly Correlated** — Active-space and CI/DMRG/FCIQMC for static correlation and near-degeneracy (bond breaking, transition metals).
- **Density Functional Theory (DFT)** — Kohn–Sham densities with approximate functionals (hybrid, meta-GGA, range-separated, double-hybrid); good cost/accuracy balance.
- **Geometry Optimization and Vibrations** — Derivative-driven minima searches and harmonic analysis for structures, IR/Raman, and thermochemistry.
- **Intermolecular / Non-Covalent** — SAPT family for clean energy decomposition of electrostatics, exchange, induction, dispersion without BSSE.
- **Excited States and Response** — TD-DFT, ADC(2), CIS/RPA linear response for vertical excitations and response properties.
- **Relativistic and Core** — X2C/DKH and ECPs to include relativistic effects and downfold core electrons.
- **Solvation and Environment** — Continuum PCM via PCMSolver for bulk solvent reaction fields.
- **Properties and Analysis** — Post-SCF expectation values, electrostatic potential, natural orbitals/populations, cube file visualization.

## Method Categories

### Ab Initio Wavefunction
- **Methods / Examples:** Hartree-Fock (HF; restricted HF (RHF); unrestricted HF (UHF); restricted open-shell HF (ROHF)), initial orbital guesses, symmetry-adapted orbitals
- **Underlying Principle:** Mean-field approximation with single Slater determinant; variational optimization of molecular orbitals.

### Post-HF Correlation (Single-Reference)
- **Methods / Examples:** Møller–Plesset perturbation theory second to fourth order (MP2 / density-fitted MP2 (DF-MP2) / domain-based local pair natural orbital MP2 (DLPNO-MP2), MP3, MP4(SDQ)), coupled-cluster with singles and doubles (CCSD), CC with perturbative triples (CCSD(T)), lambda-augmented CC with perturbative triples (Λ-CCSD(T)), orbital-optimized MP2 / orbital-optimized coupled-cluster (OO-MP2 / OO-CC), frozen natural orbital (FNO) variants, coupled electron pair approximation (CEPA), quadratic configuration interaction with singles and doubles plus perturbative triples (QCISD(T))
- **Underlying Principle:** Systematic inclusion of dynamic electron correlation via perturbation theory (MPn) or exponential ansatz (coupled-cluster) for size-consistent, high-accuracy energies beyond mean-field.

### Multi-Reference / Strongly Correlated
- **Methods / Examples:** Multiconfigurational self-consistent field (MCSCF) / complete active space self-consistent field (CASSCF), configuration interaction (CI) singles and doubles (CISD), CI singles doubles triples (CISDT), full CI via determinant-based CI (detCI), interfaces to external density matrix renormalization group (DMRG) / full configuration interaction quantum Monte Carlo (FCIQMC)
- **Underlying Principle:** Multi-determinant wavefunctions to capture static correlation and near-degeneracies (e.g., bond breaking, transition metals, conical intersections).

### Density Functional Theory (DFT)
- **Methods / Examples:** Hybrid, meta-generalized gradient approximation (meta-GGA), range-separated, double-hybrid functionals (via Libxc), time-dependent DFT (TD-DFT), non-local correlation functionals (DFT-NL), dispersion corrections (Grimme DFT-D3 / D4, VV10), density cumulant theory (DCT)
- **Underlying Principle:** Kohn-Sham framework with approximate exchange-correlation functionals for efficient inclusion of correlation at lower formal scaling than wavefunction methods.

### Geometry Optimization & Vibrations
- **Methods / Examples:** Analytic gradients and Hessians, quasi-Newton / conjugate-gradient / rational function optimization (RFO) optimizers, harmonic frequency analysis, infrared (IR) and Raman intensities, thermochemistry
- **Underlying Principle:** Energy landscape exploration via first/second derivatives; normal-mode analysis for vibrational spectra and zero-point / thermal corrections.

### Intermolecular / Non-Covalent Interactions
- **Methods / Examples:** Symmetry-Adapted Perturbation Theory (SAPT0, SAPT2, SAPT2+, SAPT2+(3), frozen-core/ionization SAPT (F/I-SAPT)), functional-group SAPT, many-body effects
- **Underlying Principle:** Perturbative decomposition of intermolecular forces (electrostatic, exchange, induction, dispersion) without supermolecular BSSE issues.

### Excited States & Response Properties
- **Methods / Examples:** Time-dependent DFT (TD-DFT), algebraic-diagrammatic construction (ADC(2), ADC(2)-x), configuration interaction singles (CIS), random phase approximation (RPA), polarizabilities, transition moments
- **Underlying Principle:** Linear-response theory to time-dependent perturbations for vertical excitations, oscillator strengths, and response properties.

### Relativistic & Core Treatments
- **Methods / Examples:** Scalar relativistic approaches (exact two-component (X2C), Douglas–Kroll–Hess (DKH)), effective core potentials (ECP), core-valence basis sets
- **Underlying Principle:** Accounting for relativistic effects in heavy elements and reducing computational cost by replacing core electrons with potentials.

### Solvation & Environment
- **Methods / Examples:** Interface to continuum solvation models such as the polarizable continuum model (PCM) via PCMSolver
- **Underlying Principle:** Effective treatment of bulk solvent effects via reaction-field or apparent surface charge approaches.

### Properties & Analysis
- **Methods / Examples:** One-electron properties (dipoles, multipoles, electrostatic potentials), natural orbitals/populations, cube file generation (densities, orbitals), orbital visualization
- **Underlying Principle:** Post-SCF evaluation of expectation values and derived quantities from wavefunctions or densities.
