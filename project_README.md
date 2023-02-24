---
title: "ng_readme"
author: "Nathan"
date: "1/30/2023"
output: html_document
---

This project utilizes three data sets that examine different parameters across a daily time series: (1) Enumeration of Vibrio, (2) Dust concentration (AOT), and (3) Temperature and Salinity  measurements.\
In order to reproduce the work from this project, one needs to follow  these two steps:\
(1) Clone this repo containing the data and code 
(2) Open and run the code found in the `wrangling_code` folder for the respective data set of interest. 
(3) Open and run the code found in the `analysis_code` folder for the respective data set of interest. \
\

The `wrangling_code` folder contains:\
- `dust_conc_processing.qmd`: Cleans up dust data from NRL 
- `total_copies_calculator.qmd`: Cleans up qPCR outputs to produce copies per mL for enumeration
\
The `analysis_code` folder contains:\
- `daily.qmd`: Looks at Vibrio enumeration over daily time series
- `dust.qmd`:Examines dust AOT across daily time series
- `dust_and_copies.qmd`: Combines dust AOT data with Vibrio enumeration
- `env_par.qmd`: Examines Temperature and Salinity across time series