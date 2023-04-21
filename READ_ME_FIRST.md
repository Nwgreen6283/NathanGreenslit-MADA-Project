---
title: "project_readme"
author: "Nathan"
date: "1/30/2023"
output: html_document
---

**NOTE:** Viewing all files in `Visual Mode` aids in understanding the layout and workflow.

This project utilizes three data sets that examine different parameters across a daily time series: (1) Enumeration of Vibrio (copies_master.csv), (2) Dust concentration (dust.csv), and (3) Environmental Parameters(ysi_2.csv). The first two are found in the raw_data folder. The third did not require cleaning and can be found in the processed_data folder. Within this folder, clean data sets of Enumeration of Vibrio (total_clean_copies), Dust Concentration (dust_clean.rds), and Environmental Parameters (ysi_2.csv) can be found. An additional manually altered data set titled dust_master.csv was made to look at different dust permutations: time points, sums, and averages of dust. This will become useful in statistical analyses.\

In order to reproduce the work from this project, one needs to follow these steps:\
(I) **CLONE**: Clone this repo containing the data and code\
\
(II) **CLEAN**: Open and run the code found in the `wrangling_code` folder for the respective data set of interest.\
- (1) run `1_dust.qmd`: Cleans up dust data from the Naval Research Lab\
- (2) run `2_total_copies_vibio.qmd`: Cleans up qPCR outputs to produce copies per mL for enumeration\
- (3) run `3_df_master.qmd`: Combines clean data frames for dust, copies, and environmental parameters.\
\
(III) **ANALYSIS**: Open and run the code found in the `analysis_code` folder for the respective data set of interest. Order does not matter.

(1) dust:

    1.  \`daily_dusts.qmd\`: interpretations of dust concentrations(sum, average, individual hours). This becomes important in statistical analysis.

    2.  dust_and_copies.qmd\`: This is nice for visualizing potential relationships between dust days and Vibrio growth.

(2) env:

    1.  env_par.qmd\`: Examines Temperature and Salinity across time series

<!-- -->

(3) qPCR:

    1.  \`daily_qmd\`: examines Vibrio enumeration over daily time series. This is also done as part of the \`daily_dusts.qmd\` code.

\
(IV) **STATISTCS**: Open and run the code found in `analysis_code/stats` folder for the respective data of interest.

(1) stats:

    1.  \`1_distributiom.qmd\`: Checks distribution of variables of interest

    2.  \`2_cca.qmd\`: Runs cross-correlation analysis to assess significant lags in timeseries data

    3.  \`3_correlation.qmd\`: Runs Correlation matrices on all variables

    4.  \`4_uni_variate.qmd\` : runs univariate models on variable and predictors of interest.

    5.  \`5_multi_variate.qmd\`: runs multivariate models on variable of interest (copies_mL)
