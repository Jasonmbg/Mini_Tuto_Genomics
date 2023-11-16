# Harnessing public genomics datasets for processing & utilizing mutational data [PART I]

##### PILOT internship project --> **ultimate evaluation of variant prioritization methods & re-utilization of available molecular information**

#### Efstathios-Iason Vlachavas
###### DKFZ-Division of Molecular Genome Analysis (B050)
###### Efstathios-Iason.Vlachavas@dkfz-heidelberg.de

### OVERVIEW OF THE PROJECT

*We will exploit the Colorectal Adenocarcinoma (MSK, Nat Commun 2022) dataset {https://doi.org/10.1038/s41467-022-35592-9} including ~180 patients with colitis-associated cancers (mainly focusing on mutations + copy-number alterations)*.

## Important R packages that need to be installed for the first part of the tutorial:

```r
packages = c("maftools","tidyverse")

if(!requireNamespace("BiocManager")) {
    install.packages("BiocManager")
}

library(BiocManager)

for(p in packages) {
    if(!requireNamespace(p)) {
        install(p)
    }
}

```
# Implementation

- Download/clone the respective github repository:
{git clone https://github.com/Jasonmbg/BRCA_Clonal_Resist_Project.git}

## Session Info 

```r
sessionInfo()
R version 4.1.0 (2021-05-18)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows 10 x64 (build 19045)

Matrix products: default

locale:
[1] LC_COLLATE=English_United States.1252  LC_CTYPE=English_United States.1252   
[3] LC_MONETARY=English_United States.1252 LC_NUMERIC=C                          
[5] LC_TIME=English_United States.1252    

attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] maftools_2.10.05 lubridate_1.9.2  forcats_1.0.0    stringr_1.5.0    dplyr_1.1.2     
 [6] purrr_1.0.1      readr_2.1.4      tidyr_1.3.0      tibble_3.2.1     ggplot2_3.4.3   
[11] tidyverse_2.0.0    

```


