# Results — Global Energy Minimum Configurations

Simulation output files from:

> Zhou, Y., Arya, G. *Discovery of two-dimensional binary nanoparticle superlattices
> using global Monte Carlo optimization.* Nature Communications 13, 7976 (2022).
> https://doi.org/10.1038/s41467-022-35690-8

---

## Contents

**Global minimum configurations** — ground-state NP structures determined by the
BHMC optimizer, corresponding to Figures 2B–E, 4A–E, and 5A–D of the paper.
Each xyz file contains the final globally stable configuration for a specific
combination of system parameters (φ, χ, ε, ω).

All files are in **xyz format**, visualizable with [OVITO](https://www.ovito.org/).

---

## File Format

Each xyz file header contains the system parameters:

```
R1=3, R2=3; Chi=0.8, Epsilon=0.04; Energy=-3.6
```

Atom labels:
- `CH4` — NP species 1 (type I)
- `H2` — NP species 2 (type II)

---

## Visualization in OVITO

1. **File → Load** → select the xyz file
2. Set particle radius to R1/R2 value from header (typically 3.0)
3. Boundary conditions: periodic in **x** and **y**, fixed in **z**
4. Color the two species differently to distinguish NP types

For full details on the algorithm and system parameters, see the main [README](../README.md).
