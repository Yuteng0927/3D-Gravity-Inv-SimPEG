**[summary](#summary) | [contents](#contents) | [usage](#usage) | [running the code](#running-the-code) | [issues](#issues) | [citations](#citations) | [license](#license)**

# 3D-Gravity-Inv-SimPEG
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4057134.svg)](https://doi.org/10.5281/zenodo.4057134)

<img src="figures/Figure5b.png" width=50% align="middle">

## Summary
This is a practice project, aiming to construct subsurface 3D density model using geophysical gravity data and the open source package [SimPEG](https://simpeg.xyz/). 

## Contents


## Usage

To run the script locally, you need to have python installed, [anaconda](https://www.anaconda.com/download/) is recommended.

- Install dependencies:
```
pip install -r requirements.txt
```

- Or, set up working environment using conda:
```
conda env create -f environment.yml
conda activate sparse-environment
```

- Install a modified version of SimPEG. Xiaolong made a few changes, yet haven't pull request so far.
```
pip install git+https://github.com/xiaolongw1223/simpeg.git@Joinv_0.13.0_gzz --upgrade --user
```

## Running the code

Download the code and unzip the file,

- In an IPython console

      run MixedLpInversion.py Input.json

- In a command terminal

      $ python MixedLpInversion.py Input.json

## Issues

Please [make an issue](https://github.com/xiaolongw1223/2020-GP-recovering-sparse-models/issues) if you encounter any problems while trying to run the notebooks.

## Citations

If you use script in your work, please cite:

Sun, J. and Wei, X., 2021. Research Note: Recovering sparse models in 3D potential‐field inversion without bound dependence or staircasing problems using a mixed Lp norm regularization. Geophysical Prospecting, 69(4), pp.901-910. [click here](https://doi.org/10.1111/1365-2478.13063)

Cockett, Rowan, Seogi Kang, Lindsey J. Heagy, Adam Pidlisecky, and Douglas W. Oldenburg. "SimPEG: An Open Source Framework for Simulation and Gradient Based Parameter Estimation in Geophysical Applications" Computers & Geosciences, September 2015. https://doi.org/10.1016/j.cageo.2015.09.015.

```
@article{Cockett2015,
author = {Cockett, Rowan and Kang, Seogi and Heagy, Lindsey J. and Pidlisecky, Adam and Oldenburg, Douglas W.},
doi = {10.1016/j.cageo.2015.09.015},
issn = {00983004},
journal = {Computers and Geosciences},
keywords = {Electromagnetics,Geophysics,Inversion,Numerical modeling,Object-oriented programming,Sensitivities},
pages = {142--154},
publisher = {Elsevier},
title = {{SimPEG: An open source framework for simulation and gradient based parameter estimation in geophysical applications}},
url = {http://dx.doi.org/10.1016/j.cageo.2015.09.015},
volume = {85},
year = {2015}
}
```

## License
This script is licensed under the [MIT License](/LICENSE) which allows academic and commercial re-use and adaptation of this work.
