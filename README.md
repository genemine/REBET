# REBET
## 1. REBET
a Method to Determine the Number of Cell Subpopulations
### 1.1 Description
REBET, is a method for determining the number of cell populations is based on gene expression profile. <br>
Two inputs are required to run REBET: (1) gene expression data matrix with samples in rows and genes in columns. (2) maximum number of clusters.

### 1.2 Download
REBET is implemented as an R package, which is freely available for non-commercial use.

[REBET_0.1.0.tar.gz](https://github.com/genemine/REBET/blob/master/REBET_0.1.0.tar.gz)

## 2. Install
Step 1: Download the above REBET package and install it in R (tested on version 3.6.0).<br>
Step 2: Install the "sva","flexclust","SC3","SingleCellExperiment","cluster","infotheo","scater","foreach","doParallel" R package (tested on version 3.6.0), which is dependent of REBET.

## 3. Usage
Notes: REBET was tested on linux.

Using REBET is very simple. Just follow the steps below:

Step 1: open your R or Rstudio. <br>
Step 2: in the R command window, run the following command to load the R package.

> library(REBET)

Step 3: in R command window, run the following command to see the help document for running REBET. Then, you should be able to see a help page.

> ?REBET

Step 4: At the end of the help page, there is an example code. Copy these codes to command to run as follows:

> data(Ramskold)

This dataset consists of gene expression values of 21042 genes from 33 samples. The true number of subpopulations is 7. <br> 
Ramsköld, D. et al. (2012). Full-length mRNA-Seq from single-cell levels of RNA and individual circulating tumor cells. Nat. Biotechnol., 30(8), 777–782.

> result = REBET(data, Kmax=10)

In general, we first set Kmax to 10, and if the estimated optimal number of clusters happens to be 10, we then increase the value of Kmax. The result is a value, which is the optimal number of cell subpopulations returned by REBET. <br>
The result returned by this example is 7, indicating that REBET accurately estimated the number of cell subpopulations in the Ramskold dataset.

## 4. Contact
If any questions, please do not hesitate to contact us at:
Hongdong Li, hongdong@csu.edu.cn

## 5. How to cite?
If you use this tool, please cite the following work.<br>
ZhaoYu Fang, Hongdong Li, QingSong Xu, REBET: a Method to Determine the Number of Cell Subpopulations, 2020, submitted
