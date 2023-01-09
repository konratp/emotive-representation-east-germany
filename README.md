# Diverging Memories: Emotive Representation of East Germany and its Communist Past in the German Bundestag


## Description of the Repository

This repository includes the underlying code and final write-up of my M.A. thesis titled "Diverging Memories: Emotive Representation of East Germany and its Communist Past in the German Bundestag." I use sentiment analysis to assess whether or not there are meaningful differences in the sentiments with which members of the German *Bundestag* refer to East Germany and its communist past.

This repository contains three main folders. The [`data_cleaning`](data_cleaning) folder contains code that cleans and preprocesses several datasets used in the main analysis, while [`main_analysis`](main_analysis) contains the code that performs the sentiment analysis as well as relevant statistical modeling. Finally, the [`thesis`](thesis) folder contains the final draft of my thesis, as submitted to the [University of Chicago's Division of the Social Sciences](https://socialsciences.uchicago.edu/) in July of 2022.


## Data

The majority of the data used in this repository comes from the Open Discourse dataset, which was assembled and published by Richter et al. in 2020. It is available through the Harvard Dataverse; [you can access it using this link](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/FIKIBO). I also utilize up-to-date geographic data provided by the Federal Statistical Office of Germany (Statistisches Bundesamt) through its *Gemeindeverzeichnis-Informationssystem* (GV-ISys). [Use this link to access the GV-ISys](https://www.destatis.de/DE/Themen/Laender-Regionen/Regionales/Gemeindeverzeichnis/Administrativ/Archiv/GVAuszugQ/AuszugGV1QAktuell.html). Finally, I chose to use the SentiMerge German-language sentiment dictionary, which can be downloaded [using this link](https://github.com/guyemerson/SentiMerge/blob/master/data/sentimerge.txt).

If you have trouble accessing any of the data or questions about my code, feel free to email me at [kpekkip@uchicago.edu](mailto:kpekkip@uchicago.edu).


## Required Packages

The packages required to load and run the contents of this repository are detailed below.

```r
library(tidyverse)
library(readxl)
library(tidytext)
library(corpus)
library(quanteda)
library(quanteda.sentiment)
library(quanteda.textplots)
library(readtext)
library(spacyr)
library(pradadata)
library(DT)
library(sandwich)
library(lmtest)
library(robustbase)
library(psych)
```