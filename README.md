# ds-toolbox-notebook-dataintegration
Contains a notebook and required files created as part of a project in the BioSS-UKCEH methods development framework. The notebook outlines methods for using Bayesian model averaging techniques to critically assess data integration approaches. 

## Repo structure
The notebook itself is found at the root of the directory under the name `data_integration_notebook.ipynb`. All of the files required to run the notebook (images, bibtex references, and BUGS models) can be found in the `Assets/` folder. 

## Repo tree
```
├── Assets/
│   ├── apa.csl
│   ├── bma.bib
│   ├── combined_model.bugs
│   ├── jags_occ_model.bugs
│   ├── n_mix_model.bugs
│   ├── Picture3.png
│   ├── state_space.dot
│   └── state_space.svg
├── CITATION.cff
├── data_integration_notebook.ipynb
├── LICENSE_CODE.md
├── LICENSE_CONTENT.md
└── README.md
```


## Requirements
* R (version $\ge$ 4.2.0) running in a standard IDE (e.g., RStudio / VS Code).
* JAGS: Standalone JAGS engine (version $\ge$ 4.3.0) and the R interface package JAGSUI.
* brms: version $\ge$ 2.20.0, which requires a functional C++ toolchain (Rtools on Windows, macOS R toolchain, or gcc/clang on Linux) along with cmdstanr (recommended) or rstan as the underlying backend engine (if using rstan, change `backend = "cmdstanr"` to `backend = "rstan"`).
* loo: version $\ge$ 2.6.0 for Pareto-smoothed importance sampling leave-one-out cross-validation (PSIS-LOO).

## Data access
* All data are simulated within the notebook, no external data is required. 

## Citing this repo
To cite this repository please use:

> Wilde, J., Addy, J., Morrison, C., & Miller, D. (2026). Evaluating the added benefits of data integration using Bayesian model comparison tools (Version 1.0.0) [Computer software]. Zenodo. https://doi.org/10.5281/zenodo.23159273