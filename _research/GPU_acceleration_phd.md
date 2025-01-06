---
collection: research
category: "Chemistry"
title: "Accelerating molecular dynamics simulation models using Graphics Processing Units (2018.1-2023.7)"
---

<!-- main body -->
------------------

**Introduction**

I worked on this research project during my Ph.D. career. Our inital goal is to accelerate the GBMV2 implicit solvent model for simulating the intrinsically disordered proteins (IDPs), in particular capturing their conformational changes. The GBMV2 implicit solvent model is considered more accurate than other implicit solvent models, due to an accurate description of molecular volume, but it is significantly slower. My research study is to use the Graphics Processing Units (GPU) to accelerate it, as well as improve their performance for the IDP simulations. I also spent time on the implementation of GPU-accelerated hybrid resolution (HyRes) protein model for the IDP simulations using the OpenMM program. 

**1. Accelerating the Generalized Born with Molecular Volume and Solvent Accessible Surface Area Implicit Solvent Model Using Graphics Processing Units**

**Abstract**: The generalized Born with molecular volume and solvent accessible surface area (GBMV2/SA) implicit solvent model provides an accurate description of molecular volume and has the potential to accurately describe the conformational equilibria of structured and disordered proteins. However, its broader application has been limited by the computational cost and poor scaling in parallel computing. Here, we report an efficient implementation of both the electrostatic and nonpolar components of GBMV2/SA on graphics processing unit (GPU) within the CHARMM/OpenMM module. The GPU-GBMV2/SA is numerically equivalent to the original CPU-GBMV2/SA. The GPU acceleration offers ~60- to 70-fold speedup on a single NVIDIA TITAN X (Pascal) graphics card for molecular dynamic simulations of both folded and unstructured proteins of various sizes. The current implementation can be further optimized to achieve even greater acceleration with minimal reduction on the numerical accuracy. The successful development of GPU-GBMV2/SA greatly facilitates its application to biomolecular simulations and paves the way for further development of the implicit solvent methodology.

<img src='https://onlinelibrary.wiley.com/cms/asset/094fd4d2-b70e-4e22-8419-d12815fc8c83/jcc26133-fig-0007-m.jpg' alt='drawing' width='500'/>

**Figure 1**. (Left) Timings of CPU- and GPU-GBMV2/SA simulations. The numbers next to the CPU-GBMV2/SA bars are the production time in ns/day, and the ratios next to the fast CPU-GBMV2/SA and GPU-GBMV2/SA are folds of speedup compared to CPU-GBMV2/SA. The production rates of GPU simulations are (in ns/day): 47.00 (3GB1), 48.96 (p53-TAD), 15.93 (1BVC), 3.52 (4AT5), 1.10 (PYK) and 0.47 (LON). (Right) Percentages of time spent in various parts of GPU-GBMV2/SA calculation, including constructing and updating the lookup table (“Lookup Table”), nonpolar energies and forces (“Nonpolar”) and electrostatic energies and forces calculations (“GBEnergies” and “GBForces”). The GPU and CPU calculations were done on one NVIDIA TITAN X (Pascal) and one core of Intel Xeon E5-2620 v4 2.10 GHz CPU, respectively.

**Reference**

Gong, X.; Chiricotto, M.; Liu, X.; Nordquist, E.; Feig, M.; Brooks, C.L.; Chen, J. Accelerating the Generalized Born with Molecular Volume and Solvent Accessible Surface Area Implicit Solvent Model Using Graphics Processing Units. **Journal of Computational Chemistry** 2020, 41 (8), 830-838. DOI: https://doi.org/10.1002/jcc.26133. [Link](https://doi.org/10.1002/jcc.26133)

**2. Toward Accurate Simulation of Coupling between Protein Secondary Structure and Phase Separation**

**Abstract**: Intrinsically disordered proteins (IDPs) frequently mediate phase separation that underlies the formation of a biomolecular condensate. Together with theory and experiment, efficient coarse-grained (CG) simulations have been instrumental in understanding the sequence-specific phase separation of IDPs. However, the widely used Cα-only models are limited in capturing the peptide nature of IDPs, particularly backbone-mediated interactions and effects of secondary structures, in phase separation. Here, we describe a hybrid resolution (HyRes) protein model toward a more accurate description of the backbone and transient secondary structures in phase separation. With an atomistic backbone and coarse-grained side chains, HyRes can semiquantitatively capture the residue helical propensity and overall chain dimension of monomeric IDPs. Using GY-23 as a model system, we show that HyRes is efficient enough for the direct simulation of spontaneous phase separation and, at the same time, appears accurate enough to resolve the effects of single His to Lys mutations. HyRes simulations also successfully predict increased β-structure formation in the condensate, consistent with available experimental CD data. We further utilize HyRes to study the phase separation of TPD-43, where several disease-related mutants in the conserved region (CR) have been shown to affect residual helicities and modulate the phase separation propensity as measured by the saturation concentration. The simulations successfully recapitulate the effect of these mutants on the helicity and phase separation propensity of TDP-43 CR. Analyses reveal that the balance between backbone and side chain-mediated interactions, but not helicity itself, actually determines phase separation propensity. These results support that HyRes represents an effective protein model for molecular simulation of IDP phase separation and will help to elucidate the coupling between transient secondary structures and phase separation.

<img src='https://pubs.acs.org/cms/10.1021/jacs.3c09195/asset/images/medium/ja3c09195_0001.gif' alt='drawing' width='500'/>

**Figure 2**. Representation, efficiency, and accuracy of HyRes-GPU. **(A)** Physical representation of the HyRes model. The backbone atoms are drawn in CPK style with carbon in cyan, nitrogen in blue, oxygen in red, and hydrogen in white. The side chain beads are illustrated by vdW spheres. **(B)** Computational efficiencies of HyRes-GPU in comparison to the same model run on CPU (that is, no SASA term) for systems of different sizes. The timing simulations were performed using either a single Xeon E5-2620 CPU core or a single Nvidia RTX 4070Ti GPU card. **(C,D)** Probability distributions of Rg and residue helicity profiles of p53-TAD (1–61) simulated using HyRes-GPU, in comparison to results from HyRes II (gray traces) and atomistic force field a99SB-disp (blue traces). The vertical dashed lines mark the average Rg values of the simulated ensembles.

**Reference**

Zhang, Y.; Li, S.; Gong, X.; Chen, J. Toward accurate simulation of coupling between protein secondary structure and phase separation. Journal of the American Chemical Society 2023, 146 (1), 342-357. DOI: https://doi.org/10.1021/jacs.3c09195. [Link](https://doi.org/10.1021/jacs.3c09195)

