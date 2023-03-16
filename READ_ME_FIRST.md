---
title: "project_readme"
author: "Nathan"
date: "1/30/2023"
output: html_document
---

This project utilizes three data sets that examine different parameters across a daily time series: (1) Enumeration of Vibrio (copies_master.csv), (2) Dust concentration (dust.csv), and (3) Environmental Parameters(ysi_2.csv). The first two are found in the raw_data folder. The third did not require cleaning and can be found in the processed_data folder. Within this folder, clean data sets of Enumeration of Vibrio (total_clean_copies), Dust Concentration (dust_clean.rds), and Environmental Parameters (ysi_2.csv) can be found. An additional manually altered data set titled dust_master.csv was made to look at different dust permutations: time points, sums, and averages of dust. This will become useful in statistical analyses.\


In order to reproduce the work from this project, one needs to follow these steps:\
(1) **CLONE**: Clone this repo containing the data and code\
\
(2) **CLEAN**: Open and run the code found in the `wrangling_code` folder for the respective data set of interest.\
- (a) run `dust.qmd`: Cleans up dust data from the Naval Research Lab\
- (b) run `total_copies_vibio.qmd`: Cleans up qPCR outputs to produce copies per mL for enumeration\
- (c) run `df_master.qmd`: Combines clean data frames for dust, copies, and environmental parameters.\
\
(3) **VISUALIZE**: Open and run the code found in the `analysis_code` folder for the respective data set of interest. Order does not matter.\
1. dust:\
- `daily_dusts.qmd`: interpretations of dust concentrations(sum, average, individual hours). This becomes important in statistical analysis.\
2. env:\
- `env_par.qmd`: Examines Temperature and Salinity across time series\
3. qPCR:\
- `daily_qmd`: examines Vibrio enumeration over daily time series. This is also done as part of the `daily_dusts.qmd` code. \
\
(4) **STATISTCS**: Open and run the code found in `analysis_code/stats` folder for the respective data of interest.\
1. stats:\
- `dust_copies_stats.qmd`: For exploring dust-vibrio-environmental parameters relationship.




