---
title: "Project - Phase III"
date: 2025-06-05
draft: false
description: "Phase II"
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