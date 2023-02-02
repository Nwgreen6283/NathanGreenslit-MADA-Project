---
title: "ng_readme"
author: "Nathan"
date: "1/30/2023"
output: html_document
---

*Background Rough Draft*
Bacteria belonging to the genus Vibrio are  marine oppurtunistic heterotrophs that are ubiquitous in nature. Species of Vibrio are known to cause diseases in humans like cholera (V. cholerae), ear and wound infections (V. alginolyticus), and in some extreme cases necrotizing fasciitis and septicemia (V. vulnificus). They have also been shown to impact marine health, causing coral bleaching (V. coralliiyticus, V. shiloi, V. alginolyticus), and shellfish and fish mortality (V. harveyi, V. parahaemolyticus, V. vulnificus). Vibrio population dynamics are primarily driven by temperature and salinity, with prime conditions between 18-30°C and salinities ranging from 15-35. 

Each year, plumes of Saharan dust travel across the Atlantic via easterly trade winds. These plumes are then deposited in the surface waters of the mid-Atlantic, Caribbean, and Gulf of Mexico. These dust aerosols harbor a wide range of fungi, bacteria, virus-like-particles, minerals, and nutrients (NO3, Fe, PO4). Addition  of these nutrients to  otherwise oligotrophic settings can result in large and rapid blooms of potentially harmful microbes. While there there is evidence of these blooms in low-nutrient settings like the Florida Keys, less is known regarding microbial response to dust input in areas with *higher baseline nutrients*.  

*Question:*
How do Saharan dust events influence Vibrio populations in high nutrient coastal waters? 

*Data Description*
Data was collected at 3 sites (Blind Oso, Canals, and Gulf) in Corpus Christi, TX before, during, and after a Saharan dust event (starting on July 7th and ending on July 19th, 2022). Sites represent a gradient in background nutrient levels (Blind Oso and Canals are high, the Gulf is low). Water samples were collected for inorganic nutrients, dissolved and particulate organic matter, and microbial analysis. Vertical profiles of salinity, temperature, pH, and dissolved oxygen were obtained using a YSI ProPlus sonde. 

Variables will include
`Temperature (°C)`
`Salinity`
`Nitrate`
`Phosphate`
`Copies/mL` : Produced using quantitative PCR. Provides gene copies of Vibrio bacteria (I am hoping to also get data about specific species)
`Dust Concentration (AOT)`: from the naval research laboratory satellite data

*What I am looking for*
I expect to see a more dramatic growth response in the Gulf (low nutrient), where the higher nutrient sites may exhibit a dampened growth response since they already have high background nutrient levels. If we still see a growth response despite already having  supportive background nutrient levels, this may suggest that there are other constituents in the dust that can elicit this response.  
Nutrients, dust input, salinity, and temperature will be the primary factors of interest.


*How I will analyze it*
- Look at Vibrio growth over time series (estimated from qPCR)
- Examine relationships between dust input and Vibrio growth
- Examine influence of site-specific environmental parameters (Temperature, Salinity, Nutrients) on growth response
- Run linear models on factors like: dust x growth and nutrients x growth
- NMDS
  

