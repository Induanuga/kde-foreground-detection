# Foreground Detection using Kernel Density Estimation

This repository implements **Kernel Density Estimation (KDE)** from scratch using NumPy and applies it to foreground–background segmentation in images.

## Overview
Foreground detection is formulated as a density estimation problem, where the background distribution is modeled and low-probability pixels are classified as foreground.

## Implementation Details
- Custom KDE class built using NumPy only
- Supported kernels:
  - Gaussian
  - Triangular
  - Uniform
- Tunable bandwidth parameter
- Efficient background sampling to reduce computation

## Methodology
1. Fit KDE on background image features
2. Estimate density for each pixel in the test image
3. Apply thresholding to obtain foreground mask
4. Analyze effect of kernel choice and bandwidth

