---
collection: research
category: "Environment"
title: "AlphaFold 3 for Per- and Polyfluoroalkyl Substances (2025.1-Now)"
---

<!-- main body -->
------------------

**1. Assessing AlphaFold 3 for Per- and Polyfluoroalkyl Substances Docking in Protein Structures**

**Abstract**: 

Per- and polyfluoroalkyl substances (PFAS) are persistent environmental pollutants that may pose health risks due to strong protein interactions. While AlphaFold 3 (AF3) was recently introduced for protein–ligand modeling with high claimed accuracy, its reliability for docking PFAS remains unclear. This study evaluates AF3′s performance in predicting protein–PFAS interactions using a curated data set from the Protein Data Bank, divided into a “Before Set” (seen during AF3 training) and an “After Set” (unseen). AF3 accurately predicts protein structures and pockets but shows reduced performance in pocket-aligned ligand predictions, achieving ∼74.5% success in “Before Set” but only ∼55.8% in “After Set”, indicative of possible overfitting. We further assess the effects of PFAS type on docking outcomes. Although AF3 accurately predicts binding pockets, it favors poses where the headgroup of environment-relevant PFAS interacts with polar or positively charged residues. This is different from another native binding mode in several cases, where the hydrophobic tail is inserted in the protein, but the headgroup is exposed to the solvent. Notably, a hybrid approach combining AF3 and Vina, especially considering multiple top-ranked poses, can improve prediction accuracy. These findings support the complementary use of AF3 and Vina for accurately modeling protein–PFAS interactions.

<img src='https://pubs.acs.org/cms/10.1021/acs.est.5c03917/asset/images/medium/es5c03917_0001.gif' alt='drawing' width='500'/>

**Figure 1**. (A,B) Success rates (%) of AF3 on the “Before Set” and “After Set”, and (C,D) comparison of AF3 with different AutoDock Vina docking strategies in terms of four different structural alignment references. Success rate is defined as the percentage of samples with a heavy-atom RMSD ≤ 0.2 nm, in terms of four different structural alignment references: protein backbone, protein pocket, ligand, and pocket-aligned ligand. (A) Percentage of successful predictions for the top-ranked pose (“Best Pose: Success (%)”). (B) Percentage of successful predictions among the top-5 ranked poses (“Top-5: Success (%)”). (C) Comparison between AF3 and Vina on the “Before Set” and “After Set”. (D) Further comparison among three Vina-based strategies across the same conditions. Average success rates are shown above each bar, with error bars representing the 95% confidence intervals. Statistical significance between the two data sets was evaluated using Welch’s t-test (*p < 0.05, **p < 0.01, and ***p < 0.001).

**Reference**

Gong, X.; Zhou, H.; Huang, Q.* Assessing AlphaFold 3 for Per- and Polyfluoroalkyl Substances Docking in Protein Structures. **Environ. Sci. Technol.** 2025. DOI: https://doi.org/10.1021/acs.est.5c03917. [Link](https://doi.org/10.1021/acs.est.5c03917)

