# BERT
## 1. BERT
a Method to Determine the Number of Cell Subpopulations
### 1.1 Description
BERT, is a method for determining the number of cell populations is based on gene expression profile. Two inputs are required to run BERT: (1) gene expression data matrix with samples in rows and genes in columns. (2) maximum number of clusters.

### 1.2 Download
BERT is implemented as an R package, which is freely available for non-commercial use.

[BERT_0.1.0.tar.gz](https://github.com/genemine/BERT/blob/master/BERT_0.1.0.tar.gz)

## 2. Install
Step 1: Download the above BERT package and install it in R (tested on version 3.6.0)

Step 2: Install the "sva","flexclust","SC3","SingleCellExperiment","cluster","infotheo","scater","foreach","doParallel" R package (tested on version 3.6.0), which is dependent of BERT.

## 3. Usage
Notes: BERT was tested on linux.

Using BERT is very simple. Just follow the steps below:

Step 1: open your R or Rstudio
Step 2: in the R command window, run the following command to load the R package

> library(BERT)

Step 3: in R command window, run the following command to see the help document for running ClusterMine. Then, you should be able to see a help page.

> ?BERT

Step 4: At the end of the help page, there is an example code. Copy these codes to command to run as follows:

> data(Ramskold)

> result = BERT(data, Kmax=3)

The result is a value, which is the optimal number of cell subpopulations returned by BERT.

## 4. Contact
If any questions, please do not hesitate to contact us at:
Hongdong Li, hongdong@csu.edu.cn

## 5. How to cite?
If you use this tool, please cite the following work.

ZhaoYu Fang, Hongdong Li, QingSong Xu, BERT: a Method to Determine the Number of Cell Subpopulations, 2020, submitted
