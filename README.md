## Dozer
**Dozer** is a lightweight R package for personalized co-expression network analysis from population-scale single cell RNA-sequencing datasets. Given a single cell RNA-seq dataset of cells from multiple subjects and phenotypic information of each subject, Dozer is able to construct subject specific co-expression networks, extract network traits, and conduct association studies between network traits and subject specific information.

**Dozer** can be downloaded and installed in R through the following R command: 

```r
## install a dependency package
install.packages("lcmix", repos="http://R-Forge.R-project.org")
## install Dozer
devtools::install_github("shanlu01/Dozer", build_vignettes = FALSE)
```
As a demonstration of the analysis pipeline, we included an example dataset and a vignette in our package. The featured analyses include identifying genes showing differential centrality and gene modules having difference in connectivity between phenotypic groups.

The vignette requires a list of packages for data processing and visualization. These packages have to be installed before building the vignette.
The dependencies for vignette include ggpubr, ggplot2, ggrepel, Rtsne, Matrix, knitr, dplyr, enrichR, limma, cluster, foreach, doParallel. It takes up to 10 mins to build the vignette. The dataset can be access through the following commend
```r
load(system.file("extdata", "Jerber_demo.rda", package = "Dozer"))
```
The vignette will be built when the "built_vignettes" option is set as TRUE. Once the vignette is built, it can be browsed throught the following command
```r
devtools::install_github("shanlu01/Dozer", build_vignettes = TRUE)
browseVignettes("Dozer")
```
You can also have a quick look of the vignette using the following [link](https://htmlpreview.github.io/?https://github.com/shanlu01/Dozer/blob/main/vignettes/introduction.html).

## Reference
S. Lu and S. Keles, "Dozer: Debiased personalized gene co-expression networks for population-scale scRNA-seq data".
