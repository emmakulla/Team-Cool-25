---
title: "Project - Phase II"
date: 2025-05-27
draft: false
description: "Phase II"
slug: "phase2post"
tags: ["project", "Setup"]
authors:
  - "sophiefarrell"
  - "johnnguyen"
  - "emmakulla"
  - "miagiargiari"
showAuthorsBadges: false
---

# Changes Since Phase 1

## User Personas
We slightly altered the backgrounds of two of our users. Now, Eura Peon is considering moving countries; Cara Day is now the owner of a daycare chain instead of a single daycare and is considering going global by opening a daycare in another country. Additionally, some of our user stories have changed. 

## Data Sources
We added a data source to the two that we started with. This dataset shows federal expenditure on family/children functions (such as birth grants, child allowances, etc.) per year in European countries. This dataset is broken down by expenditure type; it is reported annually and has multiple years. 

Description of data source:  
The structure of the data:
- Dimensions: benefit expenditure type, country, year
- Units: Million Euro
- Observations: Many datapoints due to multi-dimensional combinations

Relevance: 

# Wireframes
## Start Page Wireframe: 
![wireframe1](/homeWireframe.jpeg)

This will be the first page users see when they open our site. It will have our logo on the sidebar, the name of our app at the top of the screen, and options for which user they want to sign in as. Each option will have the picture of the user, their name, and a short description of them. 

## Paul E. Tishan Wireframes: 
![wireframe2](/birthPredictorWireframe.jpeg)

This screen will be shown after the user logs in as Paul E. Tishan and chooses to use the birth rate predictor. There will be a picture that represents Paul E. Tishan on the sidebar as well as the options to go back home, visit our about section, and logout. There are a lot of different inputs the user can adjust to change the predicted birth rate shown towards the bottom of the screen. Paul will use this to see what policy changes his country can make to increase birth rates, such as increasing the amount parents can receive in daycare grants. 

![wireframe3](/legislationWireframe.jpeg)

This screen will be shown after the user logs in as Paul E. Tishan and chooses the legislation finder. The user can change the country with a dropdown menu. This will cause the graph on the right to show that country's birth rate over time and cause different laws that country has made regarding focus areas that affect birth rate. Focus areas include social protection benefits, birth grants, daycare grants, etc. The user can also change the focus area in order to filter the laws so they only show legislation passed about that specific focus. 

## Cara Day Wireframes: 
![wireframe4](/businessWireframe.jpeg)

This screen will be shown after the user logs in as Cara Day and chooses business planning. The user can choose which country they want to see information about and what year in case they want to look at historical data. They can choose a store location so they can set/update the opening and closing times for that location, as well as set the cost that parent pay each month for their child to go to the daycare. I am considering adding in a "Add New Location" button so that the user can add a store in a new country like Cara Day is considering doing. 

![wireframe5](/parentResearchWireframe.jpeg)

This screen will be shown after the user logs in as Cara Day and chooses parent research. The user can select a country and different articles about things that trouble parents will be shown. The articles will show the name of the article, the author, the date it was published, and a link to the article. 

## Eura Peon Wireframes: 
![wireframe6](/countryPredictorWireframe.jpeg)

This screen will be shown after the user logs in as Eura Peon and chooses country predictor. The user can adjust the weekly hours they'd prefer to work, select the benefits they find most important (ex: day care grants, birth grants, etc.), toggle on/off if they care about the birth rate of a country, and select the year in the future they want to get their top 3 for. This will generate the top 3 countries based on their inputs. By clicking on the country, the user will get a small paragraph about the country. This screen may also be able to be used for Cara Day when looking for the best location for her new store, but as of now it is designed for Eura Peon. 

![wireframe7](/resourceFinderWireframe.jpeg)

This screen will be shown after the user logs in as Eura Peon and chooses resource finder. The user can input the country and focus area (ex: single mothers, working mothers, women in STEM, etc.) for the resources they would like to see. Then a list of resources will be generated, including helpful articles, charities that donate to the focus area inputted, afinity groups related to the focus group, etc. Each resource listed will be able to show the country it is from/in, when it was founded/published, what focus area it is under, and a link to the resource. 

# Data Cleaning


# Data Visualization

![Eura Pean Average Public Cash Benefits for Family Function per Person By Country](/CashBenEU_BAR.png)

The bar chart showing average public cash benefits per person reveals that Poland ranks significantly lower than many other EU countries in terms of financial support for families. For Eura Pean, a single woman in Warsaw considering adopting a child, this result directly impacts her decision-making. Seeing that countries like Luxembourg, Germany, and the Netherlands offer far higher levels of cash benefits, Eura may feel that Poland’s support system could leave her financially strained, especially while managing a demanding job. These results provide her with evidence that relocating to a country with more generous parental support could make raising a child more financially feasible and secure, helping her weigh the true cost of parenthood as a single mother.

![Cara Day Birth Rate vs. Childcare Expenditure per Person by Country-Year](/BirthRateCARA_SCATTER.png)

This graph is a good and valuable tool for Cara Day because she is considering expanding her business to other countries. By plotting each country’s average public childcare expenditure per person against its birth rate for multiple years, the visualization lets Cara identify where family support systems are strongest. Countries positioned in the upper right corner of the graph—those with higher birth rates and greater investment in childcare like Denmark—signal markets with growing or stable populations of young children and supportive government policies. These are the best environments for a daycare business to thrive. Conversely, countries with low birth rates and minimal public spending on childcare may not offer sustainable opportunities for expansion. Additionally, because each data point is color-coded by year, Cara can observe trends over time, like whether countries are increasing investment or experiencing declining birth rates. This time-sensitive insight helps her anticipate future demand and align her business strategy accordingly. Ultimately, the graph empowers Cara to make informed, data-driven decisions about where to grow her daycare business based on real demographic and policy patterns across Europe.

# ER Diagrams

No matter if our users want to grasp the current climate as a to-be parent, understand as a daycare operator, propose legislation as a politician, the data structure of our app seeks to help them understand their decisions that transforms their own life, those in their community, or the European Union’s ~450 million people.

## Eura Pean: Expecting Parent
![Eura Pean ER Diagram](/P2_ER_EuraPean.png)

## Cara Day: Daycare Chain Operator
![Cara Day ER Diagram](/P2_ER_CaraDay.png)

## Paul E. Tishan: EU Politician
![Paul E. Tishan ER Diagram](/P2_ER_PaulETishan.png)

## All Together: Harmonious Global ER Diagram
![Global ER Diagram](/P2_ER_Global.png)

# DDL


# ML Proof of Concept