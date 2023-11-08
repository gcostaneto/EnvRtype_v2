#  [EnvRtype:](https://github.com/allogamous/EnvRtype/blob/master/README.md) - Envirotype
<img align="left" src="/fig/logo3_300.png" width="20%" height="20%">

### A R package to interplay quantitative genomics and enviromics


#### **Current Version**: 1.2.0 (1st Dec 2023)

Last Versions: 1.1.0 (1st June 2022),  1.0.0 (31th August 2021, G3 paper version)

<div id="menu" />
  
  [![DOI](https://img.shields.io/badge/DOI-doi.org%2F10.1093%2Fg3journal%2Fjkab040-orange)](https://doi.org/10.1093/g3journal/jkab040)
  [![SUPPORT](https://img.shields.io/badge/SUPPORT-R-yellowgreen)](https://github.com/gcostaneto/EnvRtype_course/blob/main/README.md)
 

  ## Overview
  
EnvRtype (pronounced as *env-R-type* or you can say just **enviRotype**) is a R package to interplay Quantitative Genetics and Ecophysiology into a *easy* way.
Since its conception in the begining of 2020, and its first publication in 2021, the envirotyping pipeline provided by EnvRtype consists in three modules (1 - Environmental Sensing, 2- Macro-Environmental Characterization and 3 - Enviromic Similarity and Phenotype Prediction). Collectively, the EnvRtyping functions generate a simple workflow to collect, process and integrates envirotyping data into several fields of agricultural research, specially for predictive breeding that may include the use of genomic x enviromic relatedness information.
  
  <img align="center" src="/fig/workflow_2.png" width="90%" height="90%">
  
 
## Install

### Using devtools in R

```{r}
library(devtools)
devtools::install_github('allogamous/EnvRtype',force=TRUE) # current version:  1.1.0 (June 2022)
# Enter one or more numbers, or an empty line to skip updates: 3
require(EnvRtype)
  ```
### Manually installing

> If the method above doesn't work, use the next lines by downloading the EnvRtype-master.zip file

```{r}
setwd("~/EnvRtype-master.zip") # ~ is the path from where you saved the file.zip
unzip("EnvRtype-master.zip") 
file.rename("EnvRtype-master", "EnvRtype") 
shell("R CMD build EnvRtype") # or system("R CMD build EnvRtype")
install.packages("EnvRtype_1.1.0.tar.gz", repos = NULL, type="source") # Make sure to use the current verision
```
**Developer & Maintence**

 * [Germano Costa Neto](https://github.com/gcostaneto), Cornell University


## What is "Envirotyping"?

Envirotyping has proven useful in identifying the non-genetic drivers of phenotypic adaptation in plants cultivaded in diverse growing conditions. Combined with phenotyping and genotyping data, the use of envirotyping data may leverage the molecular breeding strategies to cope with environmental changing scenarios. Over the last ten years, this data has been incorporated in genomic-enabled prediction models aiming to better model genotype x environment interaction (GE) as a function of reaction-norm. However, there is difficult for most breeders to deal with the interplay between envirotyping, ecophysiology, and genetics. 
  
It also can be useful for several fields of agricultural, livestook and ecology research, by delivering high-quality environmental information and environmental grouping appraoches.

Here we present the EnvRtype R package as a new toolkit developed to facilitate the interplay between envirotyping and fields of plant research such as genomic prediction. This package offers three modules: (1) collection and processing data set, (2) environmental characterization, (3) build of ecophysiological enriched predictive models accounting for three different structures of reaction-norm over different sources of genomic relatedness. Thus, EnvRtype is useful for exploratory purposes and predctive breeding for multiple growing conditions.

<div id="menu" />
