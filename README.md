# REBET
## 1. REBET
a Method to Determine the Number of Cell Subpopulations
### 1.1 Description
REBET, is a method for determining the number of cell populations is based on gene expression profile. Two inputs are required to run REBET: (1) gene expression data matrix with samples in rows and genes in columns. (2) maximum number of clusters.

### 1.2 Download
REBET is implemented as an R package, which is freely available for non-commercial use.

[REBET_0.1.0.tar.gz](https://github.com/genemine/REBET/blob/master/REBET_0.1.0.tar.gz)

## 2. Install
Step 1: Download the above REBET package and install it in R (tested on version 3.6.0)

Step 2: Install the "sva","flexclust","SC3","SingleCellExperiment","cluster","infotheo","scater","foreach","doParallel" R package (tested on version 3.6.0), which is dependent of REBET.

## 3. Usage
Notes: REBET was tested on linux.

Using REBET is very simple. Just follow the steps below:

Step 1: open your R or Rstudio \br
Step 2: in the R command window, run the following command to load the R package

> library(REBET)

Step 3: in R command window, run the following command to see the help document for running REBET. Then, you should be able to see a help page.

> ?REBET

Step 4: At the end of the help page, there is an example code. Copy these codes to command to run as follows:

> data(Ramskold)

> result = REBET(data, Kmax=3)

The result is a value, which is the optimal number of cell subpopulations returned by REBET.

## 4. Contact
If any questions, please do not hesitate to contact us at:
Hongdong Li, hongdong@csu.edu.cn

## 5. How to cite?
If you use this tool, please cite the following work.

ZhaoYu Fang, Hongdong Li, QingSong Xu, REBET: a Method to Determine the Number of Cell Subpopulations, 2020, submitted
