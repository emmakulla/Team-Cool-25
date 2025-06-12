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



# Phase 4

## Data Model



## ML Models
In this phase, we fully implemented our second machine learning model, which was a recommendation model made for our day care owner and to be parent. In previous phases, we created a proof of concept and very rough skeleton code. In this phase however, we fully sought it through and made the concept work in the app as well. We experimented with a few different ways to create the recommendation model, and landed on using cosine similarity to match user preferences to normalized country-level statistics. Because of this, every new user input dynamically produces updated results, which shows as a ranked top 5 list of best countries that matches the user's preferences. For the day care user, it also shows a bar graph with market fit scores by country as well as a full analysis on all of the country's similarity scores. For the to-be parent, it shows a comparison bar chart of match scores by country, a plot of feature comparisons across top countries, as well as a choropleth heat map showing country's match scores. This real-time matching approach allowed us to continuously test the model’s behavior without a train-test split.



## App In Action