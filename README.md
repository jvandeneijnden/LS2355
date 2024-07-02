[![DOI](https://zenodo.org/badge/821244259.svg)](https://zenodo.org/doi/10.5281/zenodo.12622045)

# Analysis reproduction repository for "Particle acceleration at the bow shock of runaway star LS 2355: non-thermal radio emission but no gamma-ray counterpart"

![Image](main.png?raw=true "image")

## Based on Van den Eijnden et al., MNRAS accepted.
The full paper and its source files are included in this repository in the PAPER folder. 

This reproduction repository contains the following folders:

### 1) ASTROMETRY: 

Used to reproduce the Gaia-based astrometry calculations from section 3.3

### 2) IMAGE_PLOTTING:

Used to reproduce all images of radio, IR, and spectral index data in the main paper.

### 3) ANALYSIS:

Used to reproduce the non-thermal and thermal calculations in the main paper, as well as plot the related figures and the radial flux density curves.
 
### Notes:

All notebooks are commented to explain the steps and reasoning behind them.

Note that all notebooks can be run without re-performing any other part of the analysis: all necessary output from other/earlier steps is included in this repository to allow the user to repeat/build upon only these aspects of the analysis. 

Several small adjustments to Figures were made after creating (sub)plots in Python, such as combining the panels or manually updating the numbering of colorbar ticks. Such instances are mentioned explicitly within the notebooks. 

### Contact and citations:

Please get in touch via email (jakobvandeneijnden.astro [at] gmail.com) or via GitHub with any questions.

If this repository is useful for your own research, in addition to citing the original paper, please consider including a note to this repository as well, for instance via its Zenodo DOI.

### Software requirements

All python analysis was performed using Python v3.10.13.

The notebooks were created using the following Python packages/versions:
 
- numpy v1.26.4
- matplotlib v3.7.2
- astropy v5.3
- aplpy v2.1.0
- scipy v1.10.1
- FITS_TOOLS v0.2

Note that, in particular, the versions of APLPY and Matplotlib are important; different (even newer!) versions may not be compatible and lead to errors. Personally, I usually define a specific Conda environment with these specific versions for image plotting purposes.