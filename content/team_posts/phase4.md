---
title: "Project - Phase IV"
date: 2025-06-12
draft: false
description: "Phase IV"
slug: "phase4post"
tags: ["project", "Setup"]
authors:
  - "sophiefarrell"
  - "johnnguyen"
  - "emmakulla"
  - "miagiargiari"
showAuthorsBadges: false
---

# Changes Since Phase 3



## Visualizations

![percapita](/CaraVizPerCapita.png)

We edited a previous visualization that was created for phase 3, which was a choropleth heatmap which showed the amounts of grants each country in the EU recieved for childcare expenditure. The edit that we made was switching it to show the amount per capita rather than the total for each country, so that the number was not just reliant on the country's population.

## Models
In regard to our models, phase four is where they truly began to take shape! We completely integrated both our models. Model one evolved from phase two, with all cubed features being removed, as well as adding a year feature, making the model predict the birth rateg for 2024. Since phase three, we have further developed all pages of our app, creating different visualizations and features to add value to our users' experience. 


# Phase 4

## Data Model



## ML Models

Model 1

Since phase 3, Model one was further refined in order to become a predictive model for the birth rates in 2024 of EU countries. This means the year feature was added, we also removed some of the squared and cubed features to adjust for the strong multicollineariy we saw in phase 3 (as reccommended by Dr. Gerber). A quick overview:

The Features:
- Average working hours
- Year
- Maternity per capita
- Services per capita
- Average working hours squared
- Cash per capita squared
- Services per capita squared

Model Evaluation:
- MAE: .8335
- R²: .1998

Model Coefficients: 
- Intercept: 9.67 
- Weekly hours: 3.43
- Maternity per capita: 0.54 
- Services per capita: -1.15
- Year: -0.46
- Weekly hours squared: -3.86
- Cash per capita squared: -1.37  
- Services per capita squared: 2.24

Assumptions:
Through adding these slight tweaks to the model and it's features, the testing of the assumptions relatively similar to what we did in phase 3. As Dr. Gerber explained, our features do still show a strong of multicollinearity, as there still are some repeated features in terms of squared/cubed values. 

Model 2

The inputs:
- Desired working hours
- Importance of benefits
- Maternity/childbirth benefits
- Cash benefits (periodic)
- Services per capita

![slidermenu](/preferences_slider.png)

This is an image of what the slider menu looks like to take the user input on their preferences.

![rankedlist](/ranked_list.png)

This shows the output of the top 5 countries that match the user's input about their preferences.

![matchdata](/country_dataML2.png)

This is an example of the data that is produced for each top 5 country that matches the user's input.








## App In Action