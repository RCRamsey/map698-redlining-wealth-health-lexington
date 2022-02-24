# redlining-wealth-health-lexington
A repo for exploring a final thesis project related to the wealth and health ripples through time formed by Redlining in Lexington, Kentucky.

<!-- TOC -->

## Table of Contents
- [Part I. Project Summary Proposal](#part-i-project-summary-proposal)  
- [Part II. Data Sources](#part-ii-data-sources)  
    - [HOLC Neighborhoods](#holc-neighborhoods)
    - [Aspects of Wealth](#aspects-of-wealth)
        - [Race & Segregation](#race-&-segregation)
        - [Median Household income](#median-houshold-income)
        - [Percent of Population in Poverty](#percent-of-population-in-poverty)
        - [Mortgage Approval Rates through time](#mortgage-approval-rates-through-time) 
        - [Percent Home Ownership today & Owner Reported Property Value Today](#percet-home-ownership-today-&-owner-reported-property-value-today)
- [Part III. Proposed Visuals](#part-iii-proposed-visuals)
    - [Visual 1](#visual-1)
- [Part IV. Objectives & User Needs](#part-iv-objectives-&-user-needs)
- [Part V. Data Processing & Storage](#part-v-data-processing-&-stograge)
- [Part VI. JS Libraries to Employ](#part-vi-js-libraries-to-employ)
- [Part VII. Relevant Tech & Hosting Platform](#part-vii-relevant-tech-&-hosting-platform)
- [Inspiration](#inspiration)
- [References](#references)  

<!-- /TOC -->

## Part I: Project Summary Proposal

Proposed Title: How Racial Capitalism Persists today in Lexington, KY
Proposed Sub-title: An exploration of 1930s Redlining Practices

Crampton indicated that *"maps are active and not passive"* and *"they frame the narrative"* (Crampton 2014). As such I propose a project to expolore the ripples left behind by the Home Owner's Loan Corporation Redlining Neighborhood Map *Narrative* of Lexington Kentucky and what *Active* results can be interpreted from the map's fingerprint. 

I want to design a map that displays various aspects of wealth of the current location of historically redlined neighborhoods because I want to find out what inequities have persisted generation to generation in order to help the user understand the impacts inherited by redlined policies in these neighborhoods through time.

As demand increases for living close to the Central Business District and it's new/improved amenities redlined neighborhoods are at risk of gentrification. It is hoped that maps such as the one I propose can inform a user so that better policies can be enacted to prevent the gentrification of these areas and increase long term resident access to benefit from these revitalized areas they have been excluded from in the past as a beginning effort toward equity.

## Part II: Data Sources

### HOLC Neighborhoods
All data mapped will be in comparison with the redlined neighborhoods of Lexington GeoJSON provided through [Mapping Inequality](https://dsl.richmond.edu/panorama/redlining/#loc=15/38.046/-84.534&city=lexington-ky&text=downloads) (Nelson, Winling, Marciano, Connolly et al.).
- Data Available as:
    - Shapefile or GeoJSON
    - Georectified Image
    - Scan jpg 

### Aspects of Wealth
Exploring wealth under the umbrella of the ability to accumulate generational wealth through time.

#### Race & Segregation
[*Race for the Population 18 years+ 2020*](https://data.census.gov/cedsci/table?q=p3&t=Race%20and%20Ethnicity&g=0500000US21067%241400000&y=2020)
- Data available to download:
    - CSV metadata
    - CSV file data
    - TXT file table title


#### Median Household income
[*S1901 Income in the past 12 months (in 2019 inflation-adjusted dollars)*](https://data.census.gov/cedsci/table?q=income&g=0500000US21067%241400000&y=2019)
- Data available to download: 
    - CSV file metadata
    - CSV file data
    - TXT file table title
    - 19.4 kb

#### Percent of Population in Poverty
[*S1701 Poverty Status in the past 12 months (ACS)*](https://data.census.gov/cedsci/table?q=s1701&g=0500000US21067%241400000&y=2019)
- Data available to download:
    - CSV File Metadata
    - CSV file data
    - TXT file table title
    - 59.7 kb

#### Mortgage Approval Rates through time 
Looking through HMDA Home mortgage disclosure act data to find. Still needs a source.

#### Percent Home Ownership today & Owner Reported Property Value Today
[*US census bureau American Community Survey DP04 2019*](https://data.census.gov/cedsci/table?q=DP04&g=0500000US21067%241400000)
- Data available to download:
- CSV file metadata
    - CSV file data
    - TXT file table title
    - 88.5 kb

## Part III. Proposed Visuals
### Mockup WireFrame 1
![GeoPandas](graphics/wireframe_proposal1.jpg)
**Figure 1.** Mockup wireframe 1st proposal for project's html look and feel with user interaction buttons labeled.

A similar project to reference was 673 4-5.

### Visual 1
Timeline of images from papers or hisotric jounral article map depictions. Articales of interest:
     - Kellogg, John. 1982. The Formation of Black Residential Areas in Lexington, Kentucky 1865-1887. Southern Historical Association. Vol 48. No 1. pp. 21-52.
    - O'Malley, Nancy. 2002. The Pursuit of Freedom The Evolution of Kinkeadtown, an African American Post-Civil War Neighborhood in Lexington, Kentucky. Winterthur Portfolio. Vol 37. No. 4. pp. 187-218.
    - Rabinowitz, Howard. 1976. From Reconstruction to Redemption in the Urban South. Journal of Urban History. Vol 2. No 2. pp 169-194
    - Kellogg, John. 1977. Negro Urban Clusters in the Posbellum South. Geographical Review. Vol 67. No 3. pp. 310-321.
    - Kendi, Ibram. 2016. Stamped from the Beginning The Definitive History of Racist Ideas in America. New York, Bold Type Books. pp 583. 

## Part IV. Objectives & User Needs

## Part V. Data Processing & Storage
## Part VI. JS Libraries to Employ
- Mapbox GL JS for loading vector tiles and smooth interaction
- D3.js to load data as CSV
- CSV converted on the fly to geoJSON with personal written JS loop
- Chroma.js potentially for color scale
- Sparkline.js potentially for tooltip specs of data or graphing

## Part VII. Relevant Tech & Hosting Platform

## Inspiration
- [ramp styling 2020 census by race](https://mtgis-portal.geo.census.gov/arcgis/apps/MapSeries/index.html?appid=2566121a73de463995ed2b2fd7ff6eb7)
- [overlap of holc designations & secondary ramp map](https://lojic.maps.arcgis.com/apps/MapSeries/index.html?appid=e4d29907953c4094a17cb9ea8f8f89de)

## References
- Crampton, J.W. 2014. The power of maps. In: Cloke, P., Crang, P., Goodwin, M. (Eds.), Introducing human geographies, 3. Hodder Education London.
- Robert K. Nelson, LaDale Winling, Richard Marciano, Nathan Connolly, et al., “Mapping Inequality,” American Panorama, ed. Robert K. Nelson and Edward L. Ayers, accessed January 25, 2022, https://dsl.richmond.edu/panorama/redlining//#loc=14/38.041/-84.526&city=lexington-ky&text=downloads
