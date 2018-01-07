![Inferno Screenshot](https://raw.githubusercontent.com/ashokapol/Inferno4Proteomics/master/Inferno_1.1.png)

Tags: Inferno, DAnTE, Genomics, Proteomics, Software, Statistics, Analysis, Analytics, Proteins, Peptides, Microarray, Tool

**Inferno** (formally known as DAnTE: Data Analysis Tool Extension) can perform various downstream analyses on large scale datasets from proteomics and genomics experiments.

Source code for **Inferno** is hosted on Github here: https://github.com/ashokapol/inferno4proteomics
***
Developed by Ashoka Polpitiya (ashoka.pol @ gmail.com)

***
### Installing Inferno
Install the latest version of R as administrator (as of 03/21/2016 it is version 3.2.4). To run R as administrator, right click on the downloaded R installation file and select 'Run as administrator' from the menu. R needs to be installed with the **SDI** display option (you are prompted for using either SDI or MDI during the installation of R. Select the customized option to install). And you also need to tell R to write its registry entries during installation (if you are prompted for that).

Then start R as administrator (right click on R icon/application and select 'Run as administrator') and type the following commands at the R prompt (you can cut and paste):
>`options(install.packages.check.source = "no")`<br>
>`install.packages(c("rscproxy","rcom"),repos="http://rcom.univie.ac.at/download",lib=.Library,type="win.binary")`<br>
>`library(rcom)`<br>
>`comRegisterRegistry()`<br>
>`installstatconnDCOM()`

This will install **statconnDCOM** and set the R environment for **Inferno**.

Then download the **Inferno executable** (see the top-left of this page for the zip file) and install it (again as administrator). The first time you run Inferno, it will install all the necessary R packages and may take few minutes to complete. 
***

Among many features of **Inferno** are:
* A set of diagnostic plots (Histograms, boxplots, correlation plots, qq-plots, peptide-protein rollup plots, MA plots, PCA plots, etc).
* Log transforming.
* Rolling up to proteins (3 methods are available).
* LOESS normalization
* Linear Regression Normalization
* Mean Centering
* Median Absolute Deviation (MAD) Adjustment across datasets
* Quantile Normalization
* Principal Component Analysis
* Partial Least Squares Analysis
* ANOVA (multi-way, unbalanced, random effects)
* Heatmaps with Hierarchical and K-means cluster options

Dependencies:

**Inferno** depends on the following:
1. MS Windows OS with .NET 2.0 framework 
2. R Statistical Environment (http://www.r-project.org/)
3. statconnDCOM server (http://rcom.univie.ac.at)

Inferno uses the following R packages (from http://cran.r-project.org/):
* amap: Another Multidimensional Analysis Package
* car: Companion to Applied Regression
* nlme: Linear and Nonlinear Mixed Effects Models
* outliers: Tests for outliers
* fpc: Fixed point clusters, clusterwise regression and discriminant plots
* pls: Partial Least Squares Regression (PLSR) and Principal Component Regression (PCR)
* MASS: Main Package of Venables and Ripley's MASS
* impute: Imputation for microarray data
* qvalue: Q-value estimation for false discovery rate control
* e1071: Misc Functions of the Department of Statistics (e1071), TU Wien
* gplots: Various R programming tools for plotting data
* ellipse: Functions for drawing ellipses and ellipse-like confidence regions
* plotrix: Various plotting functions
* scatterplot3d: 3D Scatter Plot
* colorspace: Colorspace Manipulation

***
License Agreement

**Inferno** is licensed under the Apache License, Version 2.0; you may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0

All publications that utilize this software should provide the citation below:

**Polpitiya AD**, Qian WJ, Jaitly N, Petyuk VA, Adkins JN, Camp DG 2nd, Anderson GA, Smith RD., DAnTE: a statistical tool for quantitative analysis of -omics data. Bioinformatics. 2008 Jul 1;24(13):1556-8. (PMID: 18453552)

![](https://raw.githubusercontent.com/ashokapol/inferno4proteomics/master/AboutInferno.png)
