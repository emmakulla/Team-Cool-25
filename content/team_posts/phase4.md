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


# Phase 4

## Data Model



## ML Models
In this phase, we fully implemented our second machine learning model, which was a recommendation model made for our day care owner and to be parent. In previous phases, we created a proof of concept and very rough skeleton code. In this phase however, we fully sought it through and made the concept work in the app as well. We experimented with a few different ways to create the recommendation model, and landed on using cosine similarity to match user preferences to normalized country-level statistics. Because of this, every new user input dynamically produces updated results, which shows as a ranked top 5 list of best countries that matches the user's preferences. For the day care user, it also shows a bar graph with market fit scores by country as well as a full analysis on all of the country's similarity scores. For the to-be parent, it shows a comparison bar chart of match scores by country, a plot of feature comparisons across top countries, as well as a choropleth heat map showing country's match scores. This real-time matching approach allowed us to continuously test the model’s behavior without a train-test split.

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