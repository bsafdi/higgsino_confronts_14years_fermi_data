# Higgsino Dark Matter Confronts 14 years of Fermi Gamma Ray Data

This repository provides the essential data products from the paper https://arxiv.org/abs/2207.10090: "Higgsino Dark Matter Confronts 14 years of Fermi Gamma Ray Data".  The paper searches for evidence of higgsino dark matter at the Galactic Center using data from the Fermi gamma-ray telescope. The analysis makes use of radial annuli centered about the Galactic Center going in steps of 1 degree from 1 degree away from the Galactic Center to 10 degrees away from the Galactic Center. In each of the annuli we perform a spectral likelihood analysis to compare the data to a signal plus background model that consists of the higgsino signal component on top of diffuse, point source, and isotropic spectral templates.  For further details of the analysis and the results, please see the paper.

This repository contains a data cube with all of the relevant likelihood evaluations for the purpose of both reproducing our results and for applying them to difference scenarios. We present the log likelihood values in each annulus as a function of the signal strength (i.e., the annihilation cross-section) and the putative higgsino mass. 

The data products are all in the `data/` folder.  The main one of interest is `LL_rad_bins_mass[i,j,k]`:
1. `i` selects the higgsino mass
2. `j` the radial bin
3. `k` the signal strength 

Additional files are provided in the data folder for interpreting these quantities.

In each annulus the annihilation cross-section has a degenerate effect on the likelihood with the J-factor. For reference, we provide the binned NFW J-factors in the data folder that go into `LL_rad_bins_mass`. Given these J-factors it is straightforward to reweight the data cube in order to consider alternate dark matter density profiles.

The jupyter notebook `jupyter/load_and_plot_data.ipynb` walks through how to load the data and compute the joint likelihood by summing over annuli. We strongly recommend referring to this notebook for additional documentation and syntax. 

Please contact the authors of https://arxiv.org/abs/2207.10090: "Higgsino Dark Matter Confronts 14 years of Fermi Gamma Ray Data" for any questions or additional data product requests.
