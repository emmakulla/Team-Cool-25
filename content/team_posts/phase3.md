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

