# MultiObjAdaptSamp
MultiObjAdaptSamp is a repository of the R code that was used in the following publication

(citation)

This R repository shows a methodology for using Gaussian processes to aid in the design of experiments for improving the accuracy of a binary classifier that is dependent on two objective criteria, ie. points that do not satisfy two different criteria are rejected.
The method also demonstrates a way of interpreting the classifier to determine how the input variables affect the classifier results.

This work is licensed under the MIT license. See LICENSE.txt for details.

## Dependencies
The program was written in R v.4.0.3 with the following packages: [dplyr](https://cran.r-project.org/web/packages/dplyr/index.html), [GPareto](https://cran.r-project.org/web/packages/GPareto/index.html), [GA](https://cloud.r-project.org/web/packages/GA/index.html)

The following additional packages are suggested. While not necessary for implementation, they were used in visualization throughout the examples: [patchwork](https://cran.r-project.org/web/packages/patchwork/index.html), [ggplot2](https://cran.r-project.org/web/packages/ggplot2/index.html)

## Citation
If you are using these adaptive sampling or classifier interpretation methods in your research, please cite the following publication:

((DOI://))

## Examples
Five test systems were studied: four purely mathematical bi-objective optimization problems and the practical case of carbon capture using quinone electrochemistry to drive pH swings. The mathematical systems are 
(1) a simple quadratic system shown in [Marler & Arora 2010](https://doi.org/10.1007/s00158-009-0460-7)
(2) a modification of that quadratic system to a quartic system with two local optima
(3) the ZDT1 function from [Zitzler, Deb, and Thiele 2000](https://doi.org/10.1162/106365600568202)
(4) a modified version of the ZDT4 function from the same paper

The 2nd and 4th examples here are compared to other machine learning methods to see how the fuzzy GP classifier compared to support vector machines and Gaussian mixtures.

The CO2 capture chemistry example was broken up into 5 different phases:
(1) Preparation (Prep): determination of the variable bounds, decoupling of correlated variables, and tuning of the objective functions, particularly the weighting function
(2) Calculations where a base was added (Ex_PCET_Basic)
(3) Calculations where an acid was added (Ex_PCET_Acidic)
(4) Exploratory calculations of Pareto front shifts with specific variables of interest (Pareto_Shifts)
(5) Post-processing (PCET_Process): aggregation of the adaptively sampled datasets from (2) and (3) to interpret variable effects and assess possible trends with real candidate compounds

Calculations for (2) and (3) were separated because the concentration of acid/base that was added spanned multiple orders of magnitude, and in order to maintain adequate resolution, we used log units for the concentration.

## Acknowledgements
This work was supervised by [Chris Gorski](https://www.engr.psu.edu/ce/enve/gorski/) in the Department of Civil and Environmental Engineering. I thank Eunhye Song (Departments of Industrial and Manufacturing Engineering) and Kostas Papakonstantinou (Civil and Environmental Engineering) at Pennsylvania State University for conversations on early conception of these methods.
