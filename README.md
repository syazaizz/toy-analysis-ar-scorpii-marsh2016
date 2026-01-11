# toy-analysis-ar-scorpii-marsh2016

# Time-Series and Toy SED Analysis of AR Scorpii

This repository contains Python notebooks reproducing the core analysis concepts from
Marsh et al. (2016), “Radio detection of the white dwarf pulsar AR Scorpii” (MNRAS 463, 2229).

The project's main focus is to understand how time-domain and broadband analyses distinguish rotation-powered white dwarf pulsars from accretion-driven variability.

# What is done here
**1. Time-series analysis (Marsh et al. (2016), Figures 2–3)**

- Simulated noisy light curve with a weak periodic signal

- Period detection using a Lomb–Scargle periodogram

- Phase folding to recover a stable pulse profile

This demonstrates how coherent periodic signals are extracted from noisy astrophysical data and why phase coherence supports a rotation-powered interpretation.

**2. Toy physical SED (Marsh et al. (2016), Figure 4)**

- Thermal blackbody emission from the M-dwarf companion

- Thermal emission from the white dwarf

- Non-thermal power-law synchrotron component

Thermal emission is modelled using the Planck function,

$$𝐵_𝜈(𝑇) = {2ℎ𝜈^3 \over 𝑐^2}  {1 \over 𝑒^{ℎ𝜈 \over 𝑘𝑇} - 1}$$

and scaled to observed fluxes via $F_v = (R/d)^2 B_v$.
The SED is plotted in $v F_v$ to show that non-thermal emission dominates the radio, consistent with Marsh et al. (2016).

# Tools

Python (NumPy, SciPy, Matplotlib)

Lomb–Scargle periodograms

Physically motivated toy models

All analysis is provided as Google Colab notebooks for full reproducibility.

# Why this matters

The workflows here mirror key techniques used in studies of white dwarf pulsars, long-period radio transients, and accreting/explosive radio sources, including radio time-series analysis and broadband spectral interpretation.

# Reference

Marsh et al. (2016), Radio detection of the white dwarf pulsar AR Scorpii
https://arxiv.org/abs/1607.08265
