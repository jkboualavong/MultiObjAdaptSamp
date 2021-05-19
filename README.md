# BayesOptTol
<<<<<<< HEAD
BayesOptTol is a repository of the R code that was used in the following publication

(citation)
=======
This R repository shows a methodology for using Gaussian processes to obtain the tolerances around multi-objective Bayesian optimization and inform which input variables are most important for study.

This work is licensed under the MIT license. See LICENSE.txt for details.

# Citing
A fully detailed description of this work can be found in the following paper:
>>>>>>> 3bbe92ee4d2a9b89d33965fa085a84de10b7a01b

This paper describes a method for using Gaussian processes to obtain the tolerances around multi-objective Bayesian optimization and inform which input variables are most important for study.

The program was written in R v.4.0.3 with the following packages: [dplyr](https://cran.r-project.org/web/packages/dplyr/index.html), GPareto

The following additional packages are suggested, but not necessary for implementation: [patchwork](https://cran.r-project.org/web/packages/patchwork/index.html), [ggplot2](https://cran.r-project.org/web/packages/ggplot2/index.html)

## Citation
If you are using this methodology in your research, please cite the following publication:

((DOI://))

## Examples
Four test systems were studied: three purely mathematical bi-objective optimization problems and the practical case of carbon capture using quinone electrochemistry to drive pH swings. The mathematical systems are (1) a simple quadratic system shown in [Marler & Arora 2010](https://doi.org/10.1007/s00158-009-0460-7), (2) a modification of that quadratic system to a quartic system with two local optima, and (3) the ZDT4 function from [Zitzler, Deb, and Thiele 2000](https://doi.org/10.1162/106365600568202).

## Acknowledgements
This work was supervised by [Chris Gorski](https://www.engr.psu.edu/ce/enve/gorski/) in the Department of Civil and Environmental Engineering and [] in the Department of XX at Pennsylvania State University.