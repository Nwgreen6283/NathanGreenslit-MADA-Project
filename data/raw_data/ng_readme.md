---
title: "ng_readme"
author: "Nathan"
date: "1/30/2023"
output: html_document
---

*Data Description*
Data was collected at 3 sites (Blind Oso, Canals, and Gulf) in Corpus Christi, TX before, during, and after a Saharan dust event (starting on July 7th and ending on July 19th, 2022). Water samples were collected for inorganic nutrients, dissolved and particulate organic matter, and microbial analysis. Vertical profiles of salinity, temperature, pH, and dissolved oxygen were obtained using a YSI ProPlus sonde. 

Variables include
`Temperature (°C)`
`Salinity`
`Nitrate`
`Phosphate`
`Copies/mL` : Produced using quantitative PCR. Provides gene copies of Vibrio bacteria
`Dust Concentration (AOT)`: from the naval reserach laboratory satellite data

*Background Rough Draft*
Bacteria belonging to the genus Vibrio are ubiquitous marine heterotrophs that are opportunistic in nature. Species of Vibrio are known to cause diseases in humans like cholera (V. cholerae), ear and wound infections (V. alginolyticus), and in some extreme cases necrotizing fascitis and septicemia (V. vulnificus). They have also been shown to impact marine health, causing coral bleaching (V. coralliiyticus, V. shiloi, V. alginolyticus), and shellfish and fish mortality (). Vibrio populations are primarily dictated by temperature and salinity, with prime conditions between 18-30°C and salinities ranging from 15-35. 

Each year, plumes of Saharan dust travel across the Atlantic via easterly trade winds. These plumes are then deposited in the surface waters of the mid-Atlantic, Caribbean, and Gulf of Mexico. These dust aerosols harbor a wide range of fungi, bacteria, virus-like-particles, minerals, and nutrients (NO3 and PO4). Addition  of these nutrients to an otherwise oligotrophic setting can result in large and rapid blooms of potentially harmful microbes. While there there is evidence of these blooms in low-nutrient settings like the Florida Keys, less is known about microbial response to dust input in areas with higher baseline nutrients.  

*Question that I am trying to answer*
How do Saharan dust events influence Vibrio populations in high nutrient coastal waters? If we still see a growth response despite already having adequate nutrients, this may suggest that there is another constiuent in the dust that is eliciting this growth response. 

*What I am looking for*
- Look at Vibrio growth over time series (qPCR)
- Examine relationships between dust input and Vibrio growth
- Exmaine influence of site-specific environmental parameters (Temperature, Salinity, Nutrients) on growth response

*How I will analyze it*
- Run linear models on factors like: dust x growth and nutrients x growth
- NMDS
  

