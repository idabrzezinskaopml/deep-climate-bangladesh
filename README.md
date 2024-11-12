# Poverty and intersecting crises in Bangladesh
This repository contains code for climate analysis in Diwakar, V., Brzezinska, I. (2024), Poverty dynamics amidst intersecting crises in rural Bangladesh, DEEP Working paper 22. Data and Evidence to End Extreme Poverty Research Programme. Available at: https://doi.org/10.55158/DEEPWP22

## Data sources:
1. [Climate Research Unit Gridded Time Series (CRU TS)](https://crudata.uea.ac.uk/cru/data/hrg/cru_ts_4.07/) on global precipitation and potential evapo-transpiration (PET) on a regular 0.5 degrees grid, from 2010 to 2020.
2. [Global Flood Database](https://global-flood-database.cloudtostreet.ai/#interactive-map), flood events in Bangladesh from 2010 to 2018.
3. [Armed Conflict Location & Event Data Project (ACLED)](https://acleddata.com/) yearly data, from 2010 to 2022.
4. [Bangladesh Integrated Household Survey (BIHS)](https://bangladesh.ifpri.info/bangladesh-integrated-household-survey/), from 2011/12 to 2019.

## Overview of scripts:

| Script  | Description |
| ------------- | ------------- |
| bangladesh_drought.Rmd | Construct Standardised Precipitation-Evapotranspiration Index (SPEI), a multi-scalar measure of drought, match household and drought data, and visualise drought in Bangladesh |
| bangladesh_flood.Rmd  | Match flood events with household data and visualise floods |
