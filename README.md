# NH3-Decomposition-Workflow
Automated density functional theory (DFT) workflow for screening first-row transition metal catalysts for ammonia decomposition.

This workflow integrates Quantum ESPRESSO (QE) with the Atomic Simulation Environment (ASE) in Python, providing a reproducible and extensible framework for:

1. Bulk unit cell relaxation
2. Slab creation and adsorbate setup
3. Adsorption energy evaluation

It was developed as part of a final-year B.Eng. Chemical Engineering research project at the University of Pretoria (2025).

# Features
- Automated bulk lattice parameter optimization (validated against literature).
- Slab construction with surface freezing options for stability.
- Adsorbate placement on slab surfaces (ontop, bridge, hollow).
- Streamlined input generation and job submission to QE.
- Automatic results storage and export (energies, CIF structures, Excel sheets).
- Error handling for SCF convergence failures in spin-polarised systems.

# Installation Requirements
This workflow can be run on Google Colab (tested environment).

## Dependencies:

- Python 3.10+
- ASE (≥3.23.0)
- NumPy
- Matplotlib
- Pandas
- Quantum ESPRESSO (pw.x, v6.8+)

Ensure to install ASE and QE in Colab

# Usage
## Step 1: Bulk relaxation

Run Step 1 (unit cell relaxation) - Journal Article.ipynb to:

- Generate bulk unit cells (Sc–Zn).
- Optimise lattice parameters.
- Save results (energies, relaxed structures).

## Step 2: Slab and adsorbates

Run Step 2 (Create and relax slab and adsorbate).ipynb to:

- Build surface slabs (bcc, fcc, hcp metals).
- Freeze lower layers for stability.
- Relax gas-phase adsorbates (NH₃, NH₂, NH, N, H).

## Step 3: Adsorption energies

Run Step 3 (Absorption Energies).ipynb to:

-Place adsorbates on slabs (ontop, bridge, hollow).
-Perform relaxation.
-Compute adsorption/desorption energies.

# Outputs

- Relaxed lattice constants.
- Relaxed slab and adsorbate structures (CIF files).
- Adsorption energies (Excel sheets, .txt summaries).
- Visualisations (plots, trajectory animations).

# References


# License

This project is licensed under the MIT License — see the LICENSE file for details.

# Contact

For questions or support, please contact:
Ruan Rabbets — ruan.rabbets@gmail.com
