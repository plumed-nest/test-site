# Imidazole Diffusion in SALEM-2 MOF

This repository contains data, analysis tools, templates, and figures from our study of imidazole diffusion through 4MR and 6MR windows in SALEM-2 MOF using OPES-enhanced machine learning potentials (DeePMD).

![Graphical abstract](TOC.png)

## Repository Structure

### `data/`
Contains processed datasets, production-grade DeePMD models, and results of molecular dynamics simulations (OPES enhanced sampling).

### `figures/`
Publication-ready figures used in the paper.

### `notebooks/`
Jupyter notebooks for data analysis, visualization, and post-processing of simulation results.

### `templates/`
Input file templates and configuration files for LAMMPS MD + PLUMED-OPES simulations. Also includes training scripts for DeePMD models.

## Citation

If you use any data, code, or resources from this repository, please cite our work as follows:

```bibtex
@article{Ethirajan2025OPES,
  year     = {2025},
  title    = {Modeling Diffusion in Metal-Organic Frameworks using On-the-fly Probability Enhanced Sampling-based Machine Learning Potentials},
  author   = {Ethirajan, Sudheesh Kumar and Kulkarni, Ambarish R},
  doi      = {10.26434/chemrxiv-2025-mg7qj-v2},
  abstract = {Machine learning potentials (MLPs) can help bridge the length- and time-scale gaps required to study diverse physicochemical phenomena in nanoporous materials with ab initio accuracy. These MLPs are typically trained on quantum chemical data obtained from traditional molecular dynamics (MD) simulations that predominantly sample near-equilibrium configurations. This often limits the model’s ability to describe high-energy, off-equilibrium states required to study rare events. To address this capability gap, we introduce a novel active learning curriculum using the On-the-fly Probability Enhanced Sampling (OPES) method. Using imidazole diffusion in the SALEM-2 metal-organic framework (MOF) as a prototypical example, we apply time-dependent OPES biases with temperature- and distance-based collective variables to systematically sample the most relevant regions of the potential energy surface. This strategy enables nanosecond-scale MD simulations with near-DFT accuracy, capturing both the expected diffusion pathway across the 6-membered window and a previously unreported ring-opening mechanism through the more constrained 4-membered window. The latter process, which involves the transient dissociation of a Zn–N bond, cannot be captured using classical force fields and is prohibitively expensive with DFT. Thus, this study highlights how enhanced sampling methods can overcome data scarcity challenges associated with training MLPs for studying rare events in nanoporous materials.}
}
```

## Contact

For questions regarding the data or methodology, please contact the corresponding author or open an issue in this repository and tag @skethirajan.
