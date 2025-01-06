---
collection: research
category: "Chemistry"
title: "Development of an accurate force field for molecular dynamics simulations (2022-Now)"
---

<!-- main body -->
------------------

**Introduction**

I constantly aim to develop the next-gernation force field across different levels of molecular dynamics (MD) simulations, including the atomistic and corase-grain models.
During my Ph.D. career, I observed that the conventional protein force fields (such as CHARMM36m) could likely have the overstabilization of charge–charge interactions.

**1. Likely Overstabilization of Charge–Charge Interactions in CHARMM36m(w): A Case for a99SB-disp Water**

**Abstract**: Recent years have witnessed drastic improvements in general-purpose explicit solvent protein force fields, partially driven by the need to study intrinsically disordered proteins (IDPs), and yet the state-of-the-art force fields such as CHARMM36m (c36m) and a99SB-disp still provide different performances in simulating disordered protein states, where c36m has a bias toward overcompaction for large IDPs. Here, we examine the performance of c36m and a99SB-disp in describing the stabilities of a set of 46 amino acid backbone and side chain pairs in various configurations. The free energy results show that c36m systematically predicts stronger interactions compared to a99SB-disp by an average of 0.2 kcal/mol for nonpolar pairs, 0.6 kcal/mol for polar pairs, and 0.8 kcal/mol for salt bridges. The most severe overstabilization in c36m is observed for charged pairs involving the Arg and Glu side chains by up to 2.9 kcal/mol. Importantly, the systematic overstabilization of c36m is only marginally alleviated by c36mw, an ad hoc patch to c36m that increases the dispersion interactions between TIP3P hydrogens and protein atoms. Guided by free energy decomposition, we evaluated if revising the charges alone could alleviate the severe overstabilization of salt bridges of c36m(w) vs a99SB-disp. The results suggested that the direct modification of protein–water interactions is also necessary. Toward this end, we proposed a tentative modification to c36m, referred to as c36mrb-disp, which combines modified Arg side chain charges, retuned backbone hydrogen bonding strength, and the a99SB-disp water model. The modified force field successfully reproduces the secondary structures of several intrinsically disordered peptides and proteins including (AAQAA)3, GB1p, and p53 transactivation domain, while maintaining the stability of a set of folded proteins. This work provides a set of useful systems for benchmarking and optimizing protein force fields and highlights the importance of balancing protein–protein and protein–water electrostatic interactions for accurately describing both folded and disordered proteins.

<img src='https://pubs.acs.org/cms/10.1021/acs.jpcb.4c04777/asset/images/medium/jp4c04777_0005.gif' alt='drawing' width='500'/>

**Figure 1**. PMF profiles of interactions of three dimers involving the glutamic acid side chain. **(A)** eks, **(B)** hpe, and **(C)** he in c36m, c36mw, a99SB-disp, and a36mrb-disp. **(D)** Summary of the stabilities of the three dimers in four force field options.

**Reference**

Gong, X.; Zhang, Y.; Chen, J. Likely Overstabilization of Charge–Charge Interactions in CHARMM36m (w): A Case for a99SB-disp Water. **The Journal of Physical Chemistry B** 2024, 128 (47), 11554–11564. DOI: https://doi.org/10.1021/acs.jpcb.4c04777. [Link](https://doi.org/10.1021/acs.jpcb.4c04777)

