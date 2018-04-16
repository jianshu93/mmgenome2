# Tools for extracting individual genomes from metagenomes
`mmgenome2` is an R-package designed to facilitate reproducible extraction of individual genomes from metagenomes. It is an implementation of the different binning strategies described in the [multi-metagenome](http://madsalbertsen.github.io/multi-metagenome/) project, and makes it possible to apply these to any metagenome data. In combination with the [RMarkdown](https://rmarkdown.rstudio.com/) format, the mmgenome2 package allows for reproducible step-by-step extraction of high-quality genomes from metagenomes as well as generating publication-ready figures with minimal effort. 

## Installation
First, install [R (3.4.3 or later)](https://mirrors.dotsrc.org/cran/) and [RStudio](https://www.rstudio.com/products/rstudio/download/#download). Windows users should also install [RTools](https://mirrors.dotsrc.org/cran/bin/windows/Rtools/). Then open RStudio as administrator (!) and run the following commands (just copy/taste) to install `mmgenome2` from the console:

```r
#check for bioconductor installer
if(!require(BiocInstaller)) 
  source("https://bioconductor.org/biocLite.R")
  
#check for devtools
if(!require(devtools))
  install.packages("devtools")
  
#install mmgenome2
BiocInstaller::biocLite("kasperskytte/mmgenome2")
```

## Get started
For a brief guide about the basics of mmgenome2 go to the [Get Started](https://kasperskytte.github.io/mmgenome2/articles/ampvis2.html) page. 