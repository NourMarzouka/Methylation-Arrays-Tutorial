# Methylation Arrays Tutorial

This tutorial provides instructions for setting up and running an analysis of methylation data using Illumina HumanMethylation EPICv2 arrays with the ChAMP package in R.
Original tutorial can be found [here](https://www.bioconductor.org/packages/release/bioc/vignettes/ChAMP/inst/doc/ChAMP.html)
## Prerequisites

Before you begin, ensure that you have the following installed on your system:

- **R**
- **RStudio**
- **Rtools** (for Windows)
- **ChAMP library**
- **ChAMPData library**

## Installing R and R Packages

### 1. Install R and RStudio

Download and install R from the [official CRAN website](https://cran.r-project.org/).  
Download and install RStudio from the [RStudio website](https://www.rstudio.com/products/rstudio/download/).

### 2. Install Rtools (Windows users only)

For Windows users, install Rtools from the [Rtools download page](https://cran.r-project.org/bin/windows/Rtools/).

### 3. Install ChAMP and ChAMPData Packages

The ChAMP and ChAMPData packages supporting on illumina HumanMethylation EPICv2 array may not be available on CRAN or BiocManager. 
Therefore, they must be installed from GitHub as [here](https://github.com/YuanTian1991/ChAMP-DemoRun/tree/main/EPICv2/illumina_demo_data_iScan)

#### Step 1: Install `devtools` Package

To enable installation of packages directly from GitHub, you need the `devtools` and `BiocManager` package. Install it using the following command:

```r
install.packages("devtools")
install.packages("BiocManager")

# load devtools
library(devtools)
library(BiocManager)
```

#### Step 2: Install `ChAMP` & `ChAMPdata` Package
```r
# ChAMPdata (>=2.31.1), and ChAMP version >= 2.29.1. 
install_github("YuanTian1991/ChAMP")
install_github("YuanTian1991/ChAMPdata")
```
