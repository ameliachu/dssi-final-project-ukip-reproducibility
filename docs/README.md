# Overview

This repository contains all of the data and code for "Does Media Coverage Drive Public Support for UKIP or Does Public Support for UKIP Drive Media Coverage?."

The entire article, the supplementary information, and all of the analyses can be reproduced by processing the file "ukip.media.Rmd" in R or (more conveniently) RStudio. This file combines all of the code and text necessary to convert the raw data sources into the published article in one step, leveraging the R package "knitr." To do so, ensure that all required packages (listed in the first code chunk in "ukip_media.Rmd") are installed on your computer, and the directory information throughout the document is updated to reflect your directories on your computer (e.g., in the setwd() functions).

If you encounter technical difficulties reproducing the entire article, "ukip_media.Rmd" is easily readable so that the code for specific analyses can be identified and extracted. It should be straightforward to manually execute only the code you need to reproduce the analyses you wish to reproduce.

# Contents

The files assume a directory containing two subdirectories:

/article
  - "ukip_media.Rmd" is the main file containing all of the text and analyses
    - "Murphy_custom.tex" is a LaTeX template (utilized by "ukip_media.Rmd")
    - "apsa.csl" is a citation stylesheet (utilized by "ukip_media.Rmd")
    - "mybib.bib" is a document containing all the references  (utilized by "ukip_media.Rmd")
    
/data 
  - "ukip_media.csv" is the main dataset containing the main monthly time-series (utilized by "ukip_media.Rmd")
  - "UKPolls" contain disaggregated polling data maintained by Jennings and co-authors (aggregated in "ukip_media.Rmd")
  - "weekly_coverage" contains the other week-level variables we gathered
  
# Instructions

Download and install R and Rstudio. Load "ukip_media.Rmd" in RStudio. Change the directory paths in the code to reflect where this replication repository is on your computer. Ensure all the required packages are installed, and "knit" the file. Your mileage may vary due to different package versions and/or other such features of your computing environment. If you experience technical difficulties, you may need to execute analyses of interest in a piecemeal fashion.