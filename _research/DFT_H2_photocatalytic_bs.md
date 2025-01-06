---
collection: research
category: "Chemistry"
title: "Accelerating a quantum chemistry VBSCF method using a Cholesky decomposition technique (2014.9-2017.7)"
---

<!-- main body -->
------------------

**Introduction**

During my M.S. program, I dedicated three years to learning quantum chemistry calculations. One of my primary projects involved accelerating the valence bond self-consistent field (VBSCF) method by implementing the Cholesky decomposition (CD) technique.

**1. The application of cholesky decomposition in valence bond calculation**

**Abstract**: The Cholesky decomposition (CD) technique, used to approximate the two-electron repulsion integrals (ERIs), is applied to the valence bond self-consistent field (VBSCF) method. Test calculations on ethylene, $C_{2n}H_{2n+2}$, and $C_{2n}H_{4n−2}$ molecules ($n$ = 1–7) show that the performance of the VBSCF method is much improved using the CD technique, and thus, the integral transformation from basis functions to VB orbitals is no longer the bottleneck in VBSCF calculations. The errors of the CD-based ERIs and of the total energy are controlled by the CD threshold, for which a value of $10^{−6}$ ensures to control the total energy error within $10^{−6}$ Hartree.

<img src='https://onlinelibrary.wiley.com/cms/asset/8829d74e-834b-439d-ae84-e58999b4de1a/jcc24442-fig-0004-m.png' alt='drawing' width='500'/>

**Figure 1**. The CPU time ratio between conventional and CD-based VBSCF calculations of $C_{2n}H_{4n−2}$ molecules, which includes **(a)** the cost of computing VBO-based ERIs, and **(b)** the total cost.

**Reference**

Gong, X.; Chen, Z.; Wu, W. The application of cholesky decomposition in valence bond calculation. **Journal of Computational Chemistry** 2016, 37 (23), 2157-2162. DOI: https://doi.org/10.1002/jcc.24442. [Link](https://doi.org/10.1002/jcc.24442)

