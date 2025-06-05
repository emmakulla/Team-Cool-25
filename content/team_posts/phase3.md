---
title: "Project - Phase III"
date: 2025-06-05
draft: false
description: "Phase III"
slug: "phase3post"
tags: ["project", "Setup"]
authors:
  - "sophiefarrell"
  - "johnnguyen"
  - "emmakulla"
  - "miagiargiari"
showAuthorsBadges: false
---

# Changes Since Phase 2



<<<<<<< HEAD
## Data Sources
We added a fourth dataset! This dataset we deemed as necessary to try and inference wether or not the expenditure given per capita is relevant when considering the cost of living in these different countries. From the advice given from our last blog post, we did see this as necessary as just because Bulgaria gives less family expenditures then Germany, it has a lower cost of living. This dataset contains annual Consumer Price Index (CPI) data for European Union countries. The CPI measures the average change over time in the prices paid by consumers for a market basket of consumer goods and services. It includes the EU27 average and individual country values and spans multiple years.

- Dimensions: Country, Year
- Units: Index value (CPI)
- Observations: Each observation is the CPI value for a specific country and year.

Relevance: This dataset is useful for understanding inflation trends across Europe. For aspiring parents or families considering relocation, the cost of living—as reflected in the CPI—can influence decisions about where to move, especially when considering the expenditures given to citizens.. Politicians and economists can use this dataset to compare how inflation varies across countries and time, and to assess how these trends may affect birth rates or the affordability of raising a child.

## ML Model Clarity
After phase two, we had certain topics to consider regarding moving forward with our models. We decided the best way to break up expenditures was into three categories: total cash expenditures, maternity expenditures (grants given for childbirth/throughout maternity), and service grants (grants for child care, at-home accommodations, etc.).

## Visualizations
Regarding our visualizations, we decided to scrap two of the three we produced last phase, only keeping and fully implementing the crude birth rate visualization. Our other two seemed to not convey useful data, so we decided to go a different route, which we will explain further.

# Phase 3
=======
# Phase 3

## REST API Matrix
| Resource | GET | PUT | POST | DELETE |
| ---------|-----|-----|------|------  |
| /locations | Gets all daycare locations from DaycareLocations (can be filtered by country) |  | Adds a new daycare location to DaycareLocations | |
| /locations{daycare_id} |  | Updates opening_time, closing_time, or monthly_price for this daycare |  | Makes this location inactive and no longer visible |
| /groups | Gets a resources from AffinityResources (can be filtered by type, country) |   | Adds a new resource to AffinityResources |   |
| /policy | Gets all policies from Poliies |   | Adds a new policy to Policies |  |
| /weeklyhours | Gets all weekly working hours (can be filtered by country)|  |  |  |
| /expenditure | Gets all expenditures from (can be filtered by type) |  |   |   |


## App In Action
![businesspage](/BusinessPlanningPage.png)
![addlocationpage](/AddNewLocation.png)


# Visualizations
## Eura Pean Employment Trends Observation

![Employment Trends Bar Graph](/EU_EMPL_.png)

This visualization was made for Eura Pean so she can observe employment trends in different countries and this will aid her in choosing a country to relocate to. This bar graph takes in three inputs, which are are gender, employment status, and country. We included hover data so when you hover your curser over a bar it will tell you the country (or if it is the EU average), as well as the average weekly working hours quantified.

## Childcare Services Expenditures by EU Country Choropleth Map

![Choropleth Map](/CaraDayExpendChoropleth.png)

The Chorpleth map generated using plot.ly shows all European Union countries and colored them coordinating with the total amount received in grants for childcare services. The more the country receives in grants the darker it is colored on the map and the color corresponds with the scale. This map will help Cara Day because it will show her which countries get the most aid for childcare, proving some to be more affordable for her needs than others.

>>>>>>> 0474dd4a701057b421add4b2d670c0de27997fd9
