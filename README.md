---
title: "project_readme"
author: "Nathan"
date: "1/30/2023"
output: html_document
---

**NOTE:** Viewing all files in `Visual Mode` aids in understanding the layout and workflow.

# Background

Each year, plumes of Saharan dust travel across the Atlantic to be deposited in the surface waters of the Caribbean and Gulf of Mexico. Dust aerosols serve as a significant source of nutrients that can elicit a fertilization effect on marine coastal waters, leading to rapid and potentially harmful blooms (e.g. red tides). Previous work has characterized the response of the marine bacteria *Vibrio* to dust input under the oligotrophic settings of the Florida Keys, but less is known regarding settings with higher baseline nutrient levels. This project aims to quantify *Vibrio* population dynamics in response to dust input in coastal sites with higher ambient nutrient levels. Daily sampling took place in Corpus Christi, TX to capture before, during, and after a Saharan dust event and quantitative PCR (qPCR) was used to estimate total counts of *Vibrio*. This study will provide an increased understanding of the conditions that can elicit potentially harmful blooms, highlighting the need for further research to understand the effects of dust deposition in non-oligotrophic waters.

# Data

This project utilizes three data sets that examine different parameters across a daily time series: (1) Enumeration of Vibrio (copies_master.csv), (2) Dust concentration (dust.csv), and (3) Environmental Parameters(ysi_2.csv). The first two are found in the raw_data folder. The third did not require cleaning and can be found in the processed_data folder. Within this folder, clean data sets of Enumeration of Vibrio (total_clean_copies), Dust Concentration (dust_clean.rds), and Environmental Parameters (ysi_2.csv) can be found. An additional manually altered data set titled dust_master.csv was made to look at different dust permutations: time points, sums, and averages of dust. This will become useful in statistical analyses.

# Reproducing this Project

In order to reproduce the work from this project, one needs to follow these steps:

### (I) **CLONE**: Clone this repo containing the data and code

### (II) **CLEAN**: Open and run the code found in the `wrangling_code` folder for the respective data set of interest.

#### (1) run `1_dust.qmd`: Cleans up dust data from the Naval Research Lab

#### (2) run `2_total_copies_vibio.qmd`: Cleans up qPCR outputs to produce copies per mL for enumeration

#### (3) run `3_df_master.qmd`: Combines clean data frames for dust, copies, and environmental parameters.

### (III) **ANALYSIS**: Open and run the code found in the `analysis_code` folder for the respective data set of interest. Order does not matter.

#### [dust]:

1.  `daily_dusts.qmd`: interpretations of dust concentrations(sum, average, individual hours). This becomes important in statistical analysis.

2.  `dust_and_copies.qmd:` This is nice for visualizing potential relationships between dust days and Vibrio growth.

#### [env]:

1.  `env_par.qmd`: Examines environmental parameters

#### [qPCR]:

1.  `daily_qmd`: examines Vibrio enumeration over daily time series. This is also done as part of the daily_dusts.qmd code.

### (IV) **STATISTCS**: Open and run the code found in `analysis_code/stats` folder for the respective data of interest.

#### [stats]:

1.  `1_distributiom.qmd\`: Checks distribution of variables of interest

2.  `2_cca.qmd\`: Runs cross-correlation analysis to assess significant lags in timeseries data

3.  `3_correlation.qmd\`: Runs Correlation matrices on all variables

4.  `4_uni_variate.qmd\` : runs univariate models on variable and predictors of interest.

5.  `5_multi_variate_models folder\`: Contains scripts that runs multivariate models on variable of interest (copies_mL) and random forest models.
