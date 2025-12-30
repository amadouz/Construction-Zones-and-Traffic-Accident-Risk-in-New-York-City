# NYC traffic crashes analysis: measuring construction-zone risk with Negative Binomial models.

## Overview
This project investigates whether active street construction is associated with higher motor-vehicle crash counts in New York City. Using NYC Open Data from 2023, the analysis focuses on crash frequency differences between construction and non-construction road segments while accounting for exposure, location, and seasonality.

## Research Question
Do road segments with active construction experience higher traffic accident rates than comparable non-construction segments?

## Data Sources
- NYC Motor Vehicle Collisions (NYPD)
- NYC Street Centerline Data (OTI)
- NYC Street Construction Permits (OTI)
(All datasets restricted to calendar year 2023)

## Methodology
- Spatially matched crashes and construction permits to street centerline segments
- Aggregated crashes at the segment–month level
- Modeled crash counts using Poisson and Negative Binomial regression
- Included segment length (km) as an exposure offset
- Controlled for borough and month effects
- Assessed overdispersion and model diagnostics

## Key Findings
- Road segments with active construction experience **over 3× higher crash rates per kilometer per month**
- Poisson regression showed severe overdispersion
- Negative Binomial regression provided a substantially better fit (AIC improvement > 80,000)
- Construction zones account for ~8% of all NYC crashes despite representing a small share of roadway segments

  ![Project cover](assets/cover.png)

## Tools & Technologies
- Python (pandas, geopandas, statsmodels)
- Spatial joins and geospatial preprocessing
- Count regression modeling
- Data visualization

## Implications
Results highlight construction zones as priority targets for traffic safety interventions, enforcement, and infrastructure planning in urban environments.

## Author
Ahmadou Diallo  
(Individual contribution from ISYE 6414 project)

