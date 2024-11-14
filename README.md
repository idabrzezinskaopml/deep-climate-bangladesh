# Poverty and intersecting crises in Bangladesh
This repository contains code for climate analysis in Diwakar, V., Brzezinska, I. (2024), Poverty dynamics amidst intersecting crises in rural Bangladesh, DEEP Working paper 22. Data and Evidence to End Extreme Poverty Research Programme. Available at: https://doi.org/10.55158/DEEPWP22

## Data sources:
1. [Climate Research Unit Gridded Time Series (CRU TS)](https://crudata.uea.ac.uk/cru/data/hrg/cru_ts_4.07/) on global precipitation and potential evapo-transpiration (PET) on a regular 0.5 degrees grid, from 1981 to 2020.
2. [Global Flood Database](https://global-flood-database.cloudtostreet.ai/#interactive-map), flood events in Bangladesh from 2010 to 2018.
3. [Armed Conflict Location & Event Data Project (ACLED)](https://acleddata.com/) yearly data, from 2010 to 2022.
4. [Bangladesh Integrated Household Survey (BIHS)](https://bangladesh.ifpri.info/bangladesh-integrated-household-survey/), from 2011/12 to 2019.
5. [Subnational administrative boundaries in Bangladesh](https://data.humdata.org/dataset/cod-ab-bgd), administrative levels 0-4 (union).
6. [Raster with national boundaries in Bangladesh](https://hub.worldpop.org/geodata/summary?id=24282), 2020.

## Overview of scripts:

| Script  | Description |
| ------------- | ------------- |
| 01_bgd_conflict_hh.Rmd | Spatially join conflict and household data |
| 02_bgd_drought  | Construct drought measure |
| 03_bgd_hh_drought_join  | Spatially join drought and household data |
| 04_bgd_hh_flood  | Spatially join flood and household data  |
| 05_bgd_climate_vis  | Visualise drought and flood  |
| 06_bgd_diff | Spatial differencing on key outcomes |

- Notes:
  Individual data files for global precipiation and evapo-transpiration for years 1981-2020 were merged into one netCDF file using the `cdo` (Climate Data Operators) package in Linux. 

