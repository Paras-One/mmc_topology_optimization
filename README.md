# MMC-Based Topology Optimization for Crashworthiness Enhancement

This repository contains the MATLAB implementation and supporting files for performing topology optimization of thin-walled structures using the **Moving Morphable Components (MMC)** method. The optimization aims to improve **crashworthiness performance** by reducing peak crushing force while maintaining sufficient energy absorption.

## 🚗 Project Overview

This study leverages the MMC-based topology optimization approach to enhance the axial crushing performance of **thin-walled square and hexagonal tubes**. The algorithm systematically searches for optimal material layouts that maximize energy absorption and crash resistance under axial loads.

Key objectives include:

- Optimizing the internal topology using MMC-based design components.
- Verifying structural performance using **ABAQUS Finite Element Analysis (FEA)**.
- Comparing different cross-sectional shapes under equivalent constraints.
- Identifying trade-offs between weight, peak crushing force, and energy absorption.

## 📊 Results Summary

### Optimized Square Tube:
- 🔻 **Weight Reduction:** 17.65%
- 🔻 **Peak Crushing Force Reduction:** 19.96%
- ⚖️ **Energy Absorption Loss:** < 16.69%

### Optimized Hexagonal Tube (same mass as optimized square tube):
- 🔺 **Energy Absorption Increase:** 8.20%
- 🔺 **Peak Crushing Force Increase:** 8.64%

These findings demonstrate that optimized hexagonal configurations can outperform traditional square tubes in energy absorption with minor trade-offs.

## 🧠 Methodology

1. **MMC-Based Topology Optimization:**
   - Randomized initial component placement.
   - Iterative material layout refinement based on crashworthiness objectives.
   - Compliance with stress constraints.

2. **Verification with ABAQUS:**
   - Final MMC designs simulated using FEM in ABAQUS.
   - Results analyzed for crash performance validation.

3. **Cross-Section Comparison:**
   - Different tube geometries tested under axial load.
   - Selection based on multi-criteria decision-making process.

## 🛠️ Tools & Technologies

- **MATLAB** – for MMC topology optimization implementation.
- **ABAQUS** – for structural FEM verification and simulation.
- **MMC Theory** – for parametric definition of design components.

## 📁 Repository Structure

```bash
mmc_topology_optimization/
│
├── mmc_optimization_code/     # MATLAB scripts for MMC-based optimization
├── abaqus_simulation/         # Input files and results from ABAQUS verification
├── plots_results/             # Post-processed results and performance graphs
└── README.md                  # Project overview and documentation
```


🧪 How to Use
-------------

1.  Clone this repo:

    ```
    git clone https://github.com/Paras-One/mmc_topology_optimization.git

    ```

2.  Open MATLAB and navigate to the `mmc_optimization_code` directory.

3.  Run the optimization script:

    ```
    run('main_optimization.m')

    ```

4.  For FEM validation, refer to the ABAQUS input files in `abaqus_simulation/`.

📚 References
-------------

If you use this work in your research or project, please consider citing or referencing the original author or methodology as inspired by MMC-based topology optimization frameworks.

🤝 Contributions
----------------

Feel free to fork the repository and contribute improvements, refactors, or simulations for other structural shapes.


