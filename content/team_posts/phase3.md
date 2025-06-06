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
| /locations/{daycare_id} |  | Updates opening_time, closing_time, or monthly_price for this daycare |  | Moves this location to a deleted locations table |
| /groups | Gets a resources from AffinityResources (can be filtered by type, country) |   | Adds a new resource to AffinityResources |   |
| /policy | Gets all policies from Poliies |   | Adds a new policy to Policies |  |
| /weeklyhours | Gets all weekly working hours (can be filtered by country)|  |  |  |
| /expenditure | Gets all expenditures from (can be filtered by type) |  |   |   |
| /m1weights | gets all the weights from the first ML model |  |  |  |

The /locations resource has two routes: one for a GET request and one for a POST request. The GET request will get all the daycare locations in the DaycareLocations table. This can be filtered by country, city, and monthly price. This route will be useful for the Cara Day persona and her business prediction page. She needs to be able to see her daycares in order to choose a location to update the opening hours, closing hours, and/or monthly price. This route could also be useful for Eura Peon on a page where she could search for a daycare in a specific country or city. 

The /locations/{daycare_id} also has two routes: one for a PUT request and one for a DELETE request. The PUT request will update the opening time, closing time, and/or monthly price of the given daycare. This route will be useful for Cara Day when changing her business' hours or price in the business planning page. The DELETE request will move the daycare to the DeletedDaycareLocations table if it shuts down or something. This will be useful for Cara Day on her business planning page as well, though it has not been implemented yet. 

The /groups resource is yet another resource with two routes: a GET request and a POST request. The GET request will get all the resources from the AffinityResource table. This can be filtered by focus area, type of resource, and country. This will be useful for the Eura Peon persona and her resources page that will connect her to different resources and affinity groups. The POST request will add a resource to the AffinityResource table in the event that Eura Peon wants to start her own affinity group or charity. 

The /policy resource also has the routes with GET and POST. The GET request will get all the legislation in the Policies table; this can be filtered by country, focus area, and year. This will be useful for Paul E. Tishian and his legislation finder page in order for the legislation to appear on the screen and for him to sort through the policies more easily. The POST request will allow him to add a new policy to the Policies table in the case that he passes a new law. 

The /weeklyhours resource has a route for GET requests; it will get all the average weekly hours from the EUEmployment table. This can be filtered by country and year. This will be useful for all of our personas, as Cara Day is interested in knowing the weekly hours so she can see which countries are best to open new locations in, Paul E Tishian is interested in weekly working hours so he can see how it effects his constituents, and Eura Peon is interested in weekly working hours so she can see which countries have better work-life balance for her potential move and new life as a mother. 

The /expenditure resource has a route for GET requests as well. This will get all the expenditures from the Children_FamilyBenefits table and can be filtered by type. This will be useful for Cara Day when she's researching new locations to open a daycare and wants to know the average daycare grants of a country. It will also be useful for Eura Peon when she wants to see which countries have the best public expenditures for parents. 


## App In Action
![businesspage](/BusinessPlanningPage.png)

This page shows off the /locations GET request route. When the "See Current Locations" button is pressed, the route is called to get the locations and put them in expanders that allows all of the information besides the daycare id and country code to be hidden until you open it. The /locations/{daycare_id} POST route can also be seen here with the "Update Price", "Update Opening Time", and "Update Closing Time" popovers that will open to show a time/number input to call the route and update these values in the database. 

![addlocationpage](/AddNewLocation.png)

This pages shows off the /locations POST request route. The user will add the attributes through the input fields and when they press the "Add Location" button it will add a row to the DaycareLocations table with the values they inputted. 

![birthratepredictor](/InitialBirthPredictor.png)

This page is our birth rate predictor, which uses our first ML model to predict the birth rate based on the different factors the user inputs. It uses the /m1weights GET request route to do so. 

# Visualizations
## Eura Pean Employment Trends Observation

![Employment Trends Bar Graph](/EU_EMPL_.png)

This visualization was made for Eura Pean so she can observe employment trends in different countries and this will aid her in choosing a country to relocate to. This bar graph takes in three inputs, which are are gender, employment status, and country. We included hover data so when you hover your curser over a bar it will tell you the country (or if it is the EU average), as well as the average weekly working hours quantified.

## Childcare Services Expenditures by EU Country Choropleth Map

![Choropleth Map](/CaraDayExpendChoropleth.png)

The Chorpleth map generated using plot.ly shows all European Union countries and colored them coordinating with the total amount received in grants for childcare services. The more the country receives in grants the darker it is colored on the map and the color corresponds with the scale. This map will help Cara Day because it will show her which countries get the most aid for childcare, proving some to be more affordable for her needs than others.

