#Radial Averaging Script for Charge Distribution and Potential Computation

## Overview
This script computes the radial average of a charge distribution from molecular dynamics simulations, using data exported in `.dx` format and converted to `.txt`. It was used in the analysis for the article:

**"Deconstructing Electrostatics of Functionalized Metal Nanoparticles from Molecular Dynamics Simulations"**

Published in *The Journal of Physical Chemistry B, Vol 127, Issue 38 (September 15, 2023)*  
Authors: *Margherita Bini, Valentina Tozzini, Giorgia Brancolini*  


## Input File Format
The script expects an input file in `.txt` format (`mappa_carica.txt`), converted from `.dx` format. The file should contain three columns representing charge density values at different grid points.

## Description of the Script
1. **Loading Data**: The script reads charge density values from the input file.
2. **Grid Setup**: Defines a 3D grid with origins and dimensions corresponding to the simulation setup.
3. **Radial Distance Calculation**: Computes the radial distance from the center of the nanoparticle (NP).
4. **Averaging Process**:
   - Partitions data into `n_interval` radial bins.
   - Computes the mean charge density and radial distance for each bin.


## Output
- `r_average`: List of average radial distances.
- `density_average`: List of corresponding charge densities.




