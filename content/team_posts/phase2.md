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
We added a data source. 

Description of data source: This dataset provides many detailed statistics on different expenditures aimed at families and children within EU member states. Itcategorizes these expenditures based off of what is provided, such as cash benefits and what kind. The data was collected annually and accessed on EUROstat.different nations. 


- Dimensions: Country, Year, Type of Benefit, Means-Testing
- Units: Monetary values presented in millions of euros, or euro per person
- Observations: Each data point represents the expenditure for a specific country, year, type of benefit, and means-testing status


Relevance: This dataset is relevant in understanding the allocation of recources towards child welfare across Europe. It can be used to assess how different countries offer family support within their social protection systems and how these benefits have changed over time. This is relevant for an aspiring parent, who might consider the different benefits countries offer for family support as possible considerations to relocate. This data is vital for politicians as well, to assess how different types of expenditure across countries correspond with birth rates.

# Wireframes
Start Page Wireframe: 
![wireframe1](/homeWireframe.jpeg)
This will be the first page users see when they open our site. It will have our logo on the sidebar, the name of our app at the top of the screen, and options for which user they want to sign in as. Each option will have the picture of the user, their name, and a short description of them. 


Paul E. Tishan Wireframes: 
![wireframe2](/birthPredictorWireframe.jpeg)
This screen will be shown after the user logs in as Paul E. Tishan and chooses to use the birth rate predictor. There will be a picture that represents Paul E. Tishan on the sidebar as well as the options to go back home, visit our about section, and logout. There are a lot of different inputs the user can adjust to change the predicted birth rate shown towards the bottom of the screen. Paul will use this to see what policy changes his country can make to increase birth rates, such as increasing the amount parents can receive in daycare grants. 

![wireframe3](/legislationWireframe.jpeg)
This screen will be shown after the user logs in as Paul E. Tishan and chooses the legislation finder. The user can change the country with a dropdown menu. This will cause the graph on the right to show that country's birth rate over time and cause different laws that country has made regarding focus areas that affect birth rate. Focus areas include social protection benefits, birth grants, daycare grants, etc. The user can also change the focus area in order to filter the laws so they only show legislation passed about that specific focus. 


Cara Day Wireframes: 
![wireframe4](/businessWireframe.jpeg)


![wireframe5](/parentResearchWireframe.jpeg)


Eura Peon Wireframes: 
![wireframe6](/countryPredictorWireframe.jpeg)

![wireframe7](/resourceFinderWireframe.jpeg)


# Data Visualization

![Eura Pean Average Public Cash Benefits for Family Function per Person By Country](/CashBenEU_BAR.png)
The bar chart showing average public cash benefits per person reveals that Poland ranks significantly lower than many other EU countries in terms of financial support for families. For Eura Pean, a single woman in Warsaw considering adopting a child, this result directly impacts her decision-making. Seeing that countries like Luxembourg, Germany, and the Netherlands offer far higher levels of cash benefits, Eura may feel that Poland’s support system could leave her financially strained, especially while managing a demanding job. These results provide her with evidence that relocating to a country with more generous parental support could make raising a child more financially feasible and secure, helping her weigh the true cost of parenthood as a single mother.

![Cara Day Birth Rate vs. Childcare Expenditure per Person by Country-Year](/BirthRateCARA_SCATTER.png)
This graph is a good and valuable tool for Cara Day because she is considering expanding her business to other countries. By plotting each country’s average public childcare expenditure per person against its birth rate for multiple years, the visualization lets Cara identify where family support systems are strongest. Countries positioned in the upper right corner of the graph—those with higher birth rates and greater investment in childcare like Denmark—signal markets with growing or stable populations of young children and supportive government policies. These are the best environments for a daycare business to thrive. Conversely, countries with low birth rates and minimal public spending on childcare may not offer sustainable opportunities for expansion. Additionally, because each data point is color-coded by year, Cara can observe trends over time, like whether countries are increasing investment or experiencing declining birth rates. This time-sensitive insight helps her anticipate future demand and align her business strategy accordingly. Ultimately, the graph empowers Cara to make informed, data-driven decisions about where to grow her daycare business based on real demographic and policy patterns across Europe.

![Paul E. Tishian Crude Birth Rate Per Country](/birthrate.png)
This line chart helps Paul by showing how birth rates have changed over time across every country, giving him a clear view of demographic trends in Europe. By tracking birth rates year by year, he can identify which countries are experiencing consistent declines, stability, or growth. This is useful for understanding how broader social or economic conditions may be influencing family planning decisions over time. It also helps Paul compare countries and consider where further analysis, such as modeling policy impacts, might be most relevant based on recent trends. Using this data, he can frame possible legislation to map that of countries who are experiencing growth in their birth rates.


















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

Model 1: Paul’s Predictive Model - Supervised
Inputs:
- Weekly Working hours
- Public expenditure 
  - Possibly refine further to include the different types of expenditure (time off, cash benefits)
Y = B0 + B1 * X1 + B2 * X2
X₁: Average weekly working hours
X₂: Expenditure
Y: Birth rate
What data will we be using: Birth rate csv, Expenditure csv, Employment hours csv
Overall: Paul would input desired weekly hours and benefit spending → the model predicts the expected birth rate for his country.

Model 2: Cara & Eura’s Recommendation Model — Unsupervised
Inputs
- Desired working hours
- Importance of benefits (e.g., child care, healthcare, parental leave)
How it works:
A weighted scoring model (or regression-style recommender):
- Each country is scored based on how well it matches the user's preferences.
What data we will be using: Birth rate csv, Expenditure csv, Employment hours csv
Steps:
- Create feature table (country-level):
  - Weekly hours, parental leave, cost of childcare, etc.
- User inputs preference weights:
  - e.g., “Childcare cost = 5 (most important), parental leave = 3, healthcare = 2…”
- Normalize data (so features are 0–1)
- Score countries:
  - Weighted sum of how well each country fits
- Rank top matches
Overall: Recommends best-fit countries to move or expand to in the future (rank based off of similarity to the features of the most desirable ideal country to live in)


# Data Cleaning
Short discussions of how we cleaned our data!

Expenditure Data Source
- In order to clean the “Public Expenditure on family/children function” API I had to remove multiple years, take out all non-EU countries and other combined rows, remove missing values, and change a lot of codes that are very Eurostat-specific. First, we took out all years before 2015 because one of the datasets we had started in 2015 and we wanted them to be easily mergeable for when we did our visualizations. Next, we removed all countries that are not in the EU so that all the datasets could be consistent. Then we standardized all of the column names and country codes paying attention to capitalization. Next, we replaced all NaN values with 0 so that it held only numerical values. We also had to save the dataset to a CSV file so that I was able to use it for my visualizations. The most time consuming of cleaning it was changing all of the Eurostat-given cryptic labels to easily readable and understandable labels, like changing “KND_CHDC” to “Childcare Services” along with fifteen other features and all twelve units because they were also in cryptic codes. 

Birth Rate Data Source
- To clean the “Live Births and Crude Birth Rate” API, we first began by removing all non-EU countries. We also took out all the years before 2015, as that is the year in which we decided to evaluate all of our datasets, as that was the furthest back that all of our datasets went. All of the birth rate data for the EU countries was there, so there were no missing values that I was working with. Finally, we just formatted the CSV into the rows: country, frequency (just annually), year, birth_rate_per_thousand, and live_births. 

Work Hours Data Source
- Cleaning the “Average number of usual weekly hours of work in main job, by sex, age, professional status, full-time/part-time and economic activity” API was a bit of a hassle. First, just like the other datasets, we removed all non-EU countries and years before 2015. A difficult part about cleaning this data was re-naming columns for clarity, such as what “nace_r2” meant in regards to employment status. We dropped rows with missing values and converted any necessary string values to floats. Overall, the dataset is still relatively large, more filtering can be done, such as removing some of the many employment statuses and refining the dataset to just what will be relevant for our personas, something that is to be determined.
