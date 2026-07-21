# Morocco and New England Zircon U-Pb Data 2024
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dyvasey/dataset-morocco-dz-2024/HEAD)

This repository consists of data and code used to analyze igneous and detrital zircon U-Pb data from Morocco and New England collected in 2024. It is primarily intended as an archive of how data analysis and figure construction were done for manuscript preparation. 

The code relies heavily on the package [geoscripts](https://github.com/dyvasey/geoscripts), which is intended for broader reusability.

## Use
### Reproducing Manuscript Figures and Tables
The code is primarily housed with Jupyter Notebooks, which are intended to be run using the conda environment specified in `environment.yml`. The easiest way to do this is by clicking the Binder badge at the top of the README and then running the individual Jupyter Notebooks. The suggested workflow to reproduce data in the manuscript on Moroccan rift tectonics submitted to _Tectonics_ is:

1. Run `process_laserchron.ipynb`, `process_ig_laserchron.ipynb`, and `process_published.ipynb` in any order. These do some initial data processing needed for the other notebooks.
2. Run `analysis_igneous.ipynb` to reproduce figures related to igneous zircon U-Pb data from Morocco
4. Run `analysis_dz.ipynb` to reproduce figures related to detrital zircon U-Pb data from Morocco.
5. Run `supp_tables.ipynb` to see construction of supplementary table of the above igneous and detrital zircon U-Pb data.

### Additional Notebooks
The other notebooks in this repository contain code used to conduct preliminary analysis and figures. These notebooks are not guaranteed to be functional or to contain usable figures/tables:
* color.ipynb
* gis_output.ipynb
* isoplotr_mds.ipynb
* map_igneous.ipynb
* map_provenance.ipynb