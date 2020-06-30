# MiRNA-QC-and-Diagnosis package

## Overview

The MiRNA-QC-and-Diagnosis (Micro RNA Quality Control and Diagnosis) is an R package to carry out training and classification analyses on datasets containing multiplets of MiRNA expression. This package contains a set of functions that implement the analysis algorithm first proposed in
> L. Ricci, V. Del Vescovo, C. Cantaloni, M. Grasso, M. Barbareschi and M. A. Denti, _Statistical analysis of a Bayesian classifier based on the expression of miRNAs_, BMC Bioinformatics __16__:287, 2015.  
DOI: [10.1186/s12859-015-0715-9](https://dx.doi.org/10.1186/s12859-015-0715-9)

Please cite this reference in works that use the present package. Citation can also be displayed in R by typing
```R
citation("MiRNAQCD")
# or, to get BibTeX items,
toBibtex(citation("MiRNAQCD"))
```

## License

This package is free software. It is distributed under the terms of the GNU General Public License (GPL), version 3.0 - see the `LICENSE.txt` file for details.
This package requires the R environment, which is free software released under the terms of GPL (see https://www.r-project.org/ for further details).
This package requires the packages `stats`, `utils`, `tools`, `pROC` and `ggplot2` (the latter two for plotting purposes). The package `devtools` is necessary if the package is installed from source.


## Authors

- Michele Castelluzzo (1) michele.castelluzzo@unitn.it
- Alessio Perinelli (1) alessio.perinelli@unitn.it
- Simone Detassis (2) simone.detassis@unitn.it
- Michela Denti (2) michela.denti@unitn.it
- Leonardo Ricci (1,3) leonardo.ricci@unitn.it

(1) Department of Physics, University of Trento, 38123 Trento, Italy.  
(2) Department of Cellular, Computational and Integrative Biology (CIBIO), University of Trento, 38123 Trento, Italy.  
(3) CIMeC, Center for Mind/Brain Sciences, University of Trento, 38068 Rovereto, Italy.

If the package turns out to be useful for your research, please cite our [paper](https://dx.doi.org/10.1186/s12859-015-0715-9):  
> L. Ricci, V. Del Vescovo, C. Cantaloni, M. Grasso, M. Barbareschi and M. A. Denti, _Statistical analysis of a Bayesian classifier based on the expression of miRNAs_, BMC Bioinformatics __16__:287, 2015. doi: [10.1186/s12859-015-0715-9](https://dx.doi.org/10.1186/s12859-015-0715-9)


## Software info

The package is available on [CRAN](https://CRAN.R-project.org/) at [https://CRAN.R-project.org/package=MiRNAQCD](https://CRAN.R-project.org/package=MiRNAQCD).  
The current package version on CRAN is __MiRNAQCD 1.0__.

The [GitHub repository](https://github.com/LeonardoRicci/MiRNA-QC-and-Diagnosis) stores the development version of the package, which typically is a few steps ahead of the CRAN release.  
The current package version on GitHub is __MiRNAQCD 1.1__.


## Documentation
The package consists in a set of functions for the R environment. All source code is under `/R/`. The package setup file (`*.tar.gz`), as well as details on how to install it, can be found within `/setup/`. See the user manual for details on the package functionalities and for setup information. Function documentation can be accessed from within R by typing
```R
help(functionName)
```
The user manual is found in `/inst/doc/manual.pdf` within the package directory tree or, once the package is installed, in `/path-to-library/MiRNAQCD/doc/manual.pdf`, where `path-to-library` can be shown within R by means of the `.libPaths()` command.


## Examples

Example code and datasets can be found in `/examples/` within the package directory tree or, once the package is installed, in `/path-to-library/MiRNAQCD/extdata/`, where `path-to-library` can be shown within R by means of the `.libPaths()` command.

The script `example_synthetic_data.R` therein contains a detailed example pipeline concerning synthetic data. The scripts `example_real_data_1.R`, `example_real_data_2.R` provide example pipelines for two real, publicly available datasets. A copy of each dataset is stored in the same folder. Example pipelines are also discussed in the user manual `/docs/manual.pdf`.


## Research

A few other works relying on the method implemented by the package:
> M. Grasso, P. Piscopo, G. Talarico, L. Ricci, A. Crestini, G. Tosto, M. Gasparini, G. Bruno, M. A. Denti, A. Confaloni, _Plasma microRNA profiling distinguishes patients with frontotemporal dementia from healthy subjects_, Neurobiology of Aging __84__:240.e1 2019. doi: [10.1016/j.neurobiolaging.2019.01.024](https://dx.doi.org/10.1016/j.neurobiolaging.2019.01.024)

> S. Detassis, V. del Vescovo, M. Grasso, S. Masella, C. Cantaloni, L. Cima, A. Cavazza, P. Graziano, G. Rossi, M. Barbareschi, L. Ricci and M. A. Denti, _miR375-3p Distinguishes Low-Grade Neuroendocrine From Non-neuroendocrine Lung Tumors in FFPE Samples_, Frontiers in Molecular Biosciences __7__:86, 2020. doi: [10.3389/fmolb.2020.00086](https://dx.doi.org/10.3389/fmolb.2020.00086)
