# Coupled Climate Variability Analysis using Canonical Correlation Analysis (CCA) 

## Overview

This project explores coupled ocean–atmosphere variability using **Canonical Correlation Analysis** (CCA), with an emphasis on both the theoretical foundations of the method and its practical application to real climate data.

- Sea Surface Temperature (SST)

- Sea Level Pressure (SLP)

The accompanying notebook provides a step-by-step explanation, from mathematical formulation to physical interpretation of the results. By combining rigorous preprocessing, dimensionality reduction, and multivariate statistical analysis, the project identifies physically meaningful coupled modes of variability, with a focus on interannual climate dynamics.

## Scientific Motivation

Climate variability is inherently multivariate: oceanic and atmospheric fields evolve together through physical feedback mechanisms.
CCA provides a natural framework to:

- Identify pairs of spatial patterns whose time evolutions are maximally correlated

- Quantify the strength of coupling between climate fields

- Interpret dominant coupled modes in a physically meaningful way

This project follows methodologies commonly used in climate dynamics and geophysical data analysis.

## Methodology

The analysis pipeline consists of the following steps:

1. Data preprocessing

- Seasonal averaging (DJFM)

- Removal of climatology

- Linear detrending

- Area weighting to account for spherical geometry

2. Dimensionality reduction

- Empirical Orthogonal Function (EOF) / PCA analysis applied separately to SST and SLP

- Truncation based on explained variance to improve numerical stability

3. Canonical Correlation Analysis

- Computation of canonical variates and canonical correlations

- Identification of leading coupled modes

4. Diagnostics and validation

- Mapping of canonical patterns (spatial correlations)

- Analysis of canonical time series

- Monte Carlo permutation significance testing

- Cross-validation to assess robustness


# Key Results

- The leading CCA mode captures a dominant coupled SST–SLP variability pattern.

- Spatial structures and time evolution are consistent with known large-scale climate modes, such as **ENSO-related ocean–atmosphere** coupling.

- Statistical testing confirms that the leading mode is **significant and robust**, not a spurious correlation.
