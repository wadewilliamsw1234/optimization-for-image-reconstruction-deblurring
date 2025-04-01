# Math 76 Final Project: Optimization Algorithms for Inverse Problems in Imaging

**Authors:** Wade Williams, Grace Faulkner, Ryan Sorkin, Isabelle Lewitt, with help from Jonathan Lindbloom  
**Date:** August 2022  

## Overview

This project compares the performance of four optimization algorithms for solving inverse problems in imaging:

- **Split-Bregman**
- **Alternating Direction Method of Multipliers (ADMM)**
- **Linearized ADMM (LADMM)**
- **Primal-Dual Hybrid Gradient (PDHG)**

The problems addressed are:
1. **MRI-like Tomographic Reconstruction**: Reconstructing an image from undersampled Fourier data.
2. **Computed Tomography (CT) Reconstruction**: Reconstructing an image from a sinogram.
3. **Image De-blurring**: Recovering a sharp image from a blurred observation.

All problems are solved using **anisotropic total variation (TV) regularization** to handle their ill-posed nature. The project utilizes the **Scientific Computational Imaging Code (SCICO)** library from Los Alamos National Laboratory for ADMM, LADMM, and PDHG implementations, while the Split-Bregman algorithm is based on Rick Archibald's MATLAB code (translated to Python).

The goal is to evaluate these algorithms in terms of reconstruction quality, convergence speed (iterations and time), and computational efficiency across the three imaging problems.

