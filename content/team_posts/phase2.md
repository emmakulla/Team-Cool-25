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
We slightly altered the backgrounds of two of our users. Now, Eura Peon is considering moving countries; Cara Day is now the owner of a daycare chain instead of a single daycare and is considering going global by opening a daycare in another country. Additionally, some of our user stories have changed. We changed two user stories for both Eura Peon and Cara Day, so now Eura's second and third user stories are different and Cara's second and fourth user stories have changed. 

## Data Sources
We added a data source to the two that we started with. This dataset shows federal expenditure on family/children functions (such as birth grants, child allowances, etc.) per year in European countries. This dataset is broken down by expenditure type; it is reported annually and has multiple years. 

Description of data source:  
The structure of the data:
- Dimensions: benefit expenditure type, country, year
- Units: Million Euro
- Observations: Many datapoints due to multi-dimensional combinations

Relevance: Helps investigate how different federal policies affect that country's birth rate. Politicians may use it to explore policy impacts of monetarily supporting parents on birth rate. Parents may use it when considering immigrating to a more financially supportive country. Daycare owners may use it to set prices within the grants their country offers parents. 

# Wireframes
## Start Page Wireframe: 
![wireframe1](/homeWireframe2.jpeg)

This will be the first page users see when they open our site. It will have our logo on the sidebar, the name of our app at the top of the screen, and options for which user they want to sign in as. Each option will have the picture of the user, their name, and a short description of them. 

## Paul E. Tishan Wireframes: 
![wireframe2](/birthRatePredictor2.jpeg)

This screen will be shown after the user logs in as Paul E. Tishan and chooses to use the birth rate predictor. There will be a picture that represents Paul E. Tishan on the sidebar as well as the options to go back home, visit our about section, and logout. There are a lot of different inputs the user can adjust to change the predicted birth rate shown towards the bottom of the screen. Paul will use this to see what policy changes his country can make to increase birth rates, such as increasing the amount parents can receive in daycare grants. 

![wireframe3](/legislationWireframe2.jpeg)

This screen will be shown after the user logs in as Paul E. Tishan and chooses the legislation finder. The user can change the country with a dropdown menu. This will cause the graph on the right to show that country's birth rate over time and cause different laws that country has made regarding focus areas that affect birth rate. Focus areas include social protection benefits, birth grants, daycare grants, etc. The user can also change the focus area in order to filter the laws so they only show legislation passed about that specific focus. 

## Cara Day Wireframes: 
![wireframe4](/businessWireframe2.jpeg)

This screen will be shown after the user logs in as Cara Day and chooses business planning. The user can choose which country they want to see information about and what year in case they want to look at historical data. They can choose a store location so they can set/update the opening and closing times for that location, as well as set the cost that parent pay each month for their child to go to the daycare. I am considering adding in a "Add New Location" button so that the user can add a store in a new country like Cara Day is considering doing. 

![wireframe5](/parentResearchWireframe2.jpeg)

This screen will be shown after the user logs in as Cara Day and chooses parent research. The user can select a country and different articles about things that trouble parents will be shown. The articles will show the name of the article, the author, the date it was published, and a link to the article. 

## Eura Peon Wireframes: 
![wireframe6](/countryPredictorWireframe2.jpeg)

This screen will be shown after the user logs in as Eura Peon and chooses country predictor. The user can adjust the weekly hours they'd prefer to work, select the benefits they find most important (ex: day care grants, birth grants, etc.), toggle on/off if they care about the birth rate of a country, and select the year in the future they want to get their top 3 for. This will generate the top 3 countries based on their inputs. By clicking on the country, the user will get a small paragraph about the country. This screen may also be able to be used for Cara Day when looking for the best location for her new store, but as of now it is designed for Eura Peon. 

![wireframe7](/resourceFinderWireframe2.jpeg)

This screen will be shown after the user logs in as Eura Peon and chooses resource finder. The user can input the country and focus area (ex: single mothers, working mothers, women in STEM, etc.) for the resources they would like to see. Then a list of resources will be generated, including helpful articles, charities that donate to the focus area inputted, afinity groups related to the focus group, etc. Each resource listed will be able to show the country it is from/in, when it was founded/published, what focus area it is under, and a link to the resource. 

# Data Visualization

![Eura Pean Average Public Cash Benefits for Family Function per Person By Country](/CashBenEU_BAR.png)

The bar chart showing average public cash benefits per person reveals that Poland ranks significantly lower than many other EU countries in terms of financial support for families. For Eura Pean, a single woman in Warsaw considering adopting a child, this result directly impacts her decision-making. Seeing that countries like Luxembourg, Germany, and the Netherlands offer far higher levels of cash benefits, Eura may feel that Poland’s support system could leave her financially strained, especially while managing a demanding job. These results provide her with evidence that relocating to a country with more generous parental support could make raising a child more financially feasible and secure, helping her weigh the true cost of parenthood as a single mother.

![Cara Day Birth Rate vs. Childcare Expenditure per Person by Country-Year](/BirthRateCARA_SCATTER.png)

This graph is a good and valuable tool for Cara Day because she is considering expanding her business to other countries. By plotting each country’s average public childcare expenditure per person against its birth rate for multiple years, the visualization lets Cara identify where family support systems are strongest. Countries positioned in the upper right corner of the graph—those with higher birth rates and greater investment in childcare like Denmark—signal markets with growing or stable populations of young children and supportive government policies. These are the best environments for a daycare business to thrive. Conversely, countries with low birth rates and minimal public spending on childcare may not offer sustainable opportunities for expansion. Additionally, because each data point is color-coded by year, Cara can observe trends over time, like whether countries are increasing investment or experiencing declining birth rates. This time-sensitive insight helps her anticipate future demand and align her business strategy accordingly. Ultimately, the graph empowers Cara to make informed, data-driven decisions about where to grow her daycare business based on real demographic and policy patterns across Europe.

# ER Diagrams

<span style="color:lightblue">Baby Blue:</span> Entity
<span style="color:red">Red:</span> Primary Key
<span style="color:yellow">Yellow:</span> Foreign Key

## Eura Pean: Expecting Parent
![Eura Pean ER Diagram](/P2_ER_EuraPean.png)
Ms. Pean is an [expecting parent](https://emmakulla.github.io/Team-Cool-25/team_posts/phase1post/#eura-pean). The ER diagram for her use case includes all data about employment, child-family benefits, and birth data across the EU and time. Her use includes an entity for `ChildcareOptions`, which she would use to compare benefits of various EU nations for expecting parents.

## Cara Day: Daycare Chain Operator
![Cara Day ER Diagram](/P2_ER_CaraDay.png)
Ms. Day is a [daycare chain operator](https://emmakulla.github.io/Team-Cool-25/team_posts/phase1post/#cara-day). The ER diagram for her use case includes all data about employment, child-family benefits, and birth data across the EU and time. Her use includes an entity for `BusinessPlanning`, which she would use to plan the `GeneralLogistics` of the service's facilities as well as plans for future `OperatingHours` with current birth rate trends.

## Paul E. Tishan: EU Politician
![Paul E. Tishan ER Diagram](/P2_ER_PaulETishan.png)
Mr. Tishan is an [EU Politician](https://emmakulla.github.io/Team-Cool-25/team_posts/phase1post/#paul-e-tishan). The ER diagram for his use case includes all data about employment, child-family benefits, and birth data across the EU and time. His use includes an entity for `PolicyAnalysis`, which he would use to plan the finances around a policy change, and details on the type, effect, and cost of the potential legislation.

## All Together: Harmonious Global ER Diagram
![Global ER Diagram](/P2_ER_Global.png)
No matter if our users want to grasp the current climate as a to-be parent, understand as a daycare operator, propose legislation as a politician, the data structure of our app seeks to help them understand their decisions that transforms their own life, those in their community, or the European Union’s ~450 million people.

# Entity-Relationship Diagram
![Global ERD Diagram](/P2_ERD_Diagram.png)
Transforming our Global ER diagram, this ERD clearly lists out the primary and foreign keys of our database design. It also incorporates data storage facilities for storing cleaned and pre-processed ML data features used for training and testing models.

# SQL DDL

Peek at our SQL DDL setup as the foundation for Eurobébé's database.

<textarea style="width: 100%; height: 200px; resize: both; overflow: auto;">
  DROP DATABASE IF EXISTS eurobebe;
  CREATE DATABASE eurobebe;
  SHOW DATABASES;
  USE eurobebe;

  -- # USER:
  -- ### User
  CREATE TABLE User
  (
      user_id    INT PRIMARY KEY,
      name       VARCHAR(50),
      age        INT,
      occupation VARCHAR(60),
      country    VARCHAR(50)
  );

  -- # DATA:
  -- ### Year
  CREATE TABLE Year
  (
      year    INT PRIMARY KEY,
      user_id INT,
      FOREIGN KEY (user_id) REFERENCES User (user_id)
          ON UPDATE cascade ON DELETE restrict
  );

  -- ### EUBirthData
  CREATE TABLE EUBirthData
  (
      eubd_id          INT PRIMARY KEY,
      country_code     VARCHAR(10),
      birth_rate       DECIMAL(5, 2),
      crude_birth_rate DECIMAL(5, 2),
      year             INT,
      FOREIGN KEY (year) REFERENCES Year (year)
          ON UPDATE cascade ON DELETE restrict
  );

  -- ### EUEmployment
  CREATE TABLE EUEmployment
  (
      eue_id            INT PRIMARY KEY,
      year              INT,
      country_code      VARCHAR(10),
      workforce         INT,
      self_employment   DECIMAL(5, 2),
      work_hours_weekly DECIMAL(5, 2),
      sex               VARCHAR(10),
      industry_sector   VARCHAR(85),
      FOREIGN KEY (year) REFERENCES Year (year)
          ON UPDATE cascade ON DELETE restrict
  );

  -- ### Children_FamilyBenefits
  CREATE TABLE Children_FamilyBenefits
  (
      cfb_id          INT PRIMARY KEY,
      year            INT,
      country_code    VARCHAR(10),
      support_program VARCHAR(85),
      dependent_type  VARCHAR(50),
      euro_amount     DECIMAL(10, 2),
      FOREIGN KEY (year) REFERENCES Year (year)
          ON UPDATE cascade ON DELETE restrict
  );

  -- # FEATURES:
  -- ## Politicians:
  -- PolicyAnalysis
  CREATE TABLE PolicyAnalysis
  (
      analysis_id  INT PRIMARY KEY,
      user_id      INT,
      country_code VARCHAR(10),
      FOREIGN KEY (user_id) REFERENCES User (user_id)
          ON UPDATE cascade ON DELETE restrict
  );

  -- ### PolicyDetails
  CREATE TABLE PolicyDetails
  (
      details_id           INT PRIMARY KEY,
      cost_per_month       DECIMAL(10, 2),
      policy_type          VARCHAR(50),
      effect_on_birth_rate DECIMAL(5, 2),
      analysis_id          INT,
      FOREIGN KEY (analysis_id) REFERENCES PolicyAnalysis (analysis_id)
          ON UPDATE cascade ON DELETE restrict
  );

  -- ## Daycare Operators:
  -- ### BusinessPlanning
  CREATE TABLE BusinessPlanning
  (
      plan_id       INT PRIMARY KEY,
      daycare_id    INT,
      year_forecast INT,
      user_id       INT,
      FOREIGN KEY (user_id) REFERENCES User (user_id)
          ON UPDATE cascade ON DELETE restrict
  );

  -- GeneralLogistics 
  CREATE TABLE GeneralLogistics
  (
      oper_id            INT PRIMARY KEY,
      staffing_demand    INT,
      financial_analysis TEXT,
      plan_id            INT,
      FOREIGN KEY (plan_id) REFERENCES BusinessPlanning (plan_id)
          ON UPDATE cascade ON DELETE restrict
  );

  -- OperatingHours 
  CREATE TABLE OperatingHours
  (
      hours_id      INT PRIMARY KEY,
      plan_id       INT,
      year_forecast INT,
      daycare_id    INT,
      FOREIGN KEY (plan_id) REFERENCES BusinessPlanning (plan_id)
          ON UPDATE cascade ON DELETE restrict
  );

  -- ## Expecting Parents:
  -- ### ChildcareOptions
  CREATE TABLE ChildcareOptions
  (
      option_id      INT PRIMARY KEY,
      country_code   VARCHAR(10),
      cost_per_month DECIMAL(10, 2),
      user_id        INT,
      FOREIGN KEY (user_id) REFERENCES User (user_id)
          ON UPDATE cascade ON DELETE restrict
  );


  -- # INSERTING TEMPORARY "DATA":
  -- ## Users (politicians, daycare operators, to-be parents)
  INSERT INTO User (user_id, name, age, occupation, country) VALUES
  (1, 'Mark Fontenot', 80, 'Politician', 'France'),
  (2, 'Eric Gerber', 80, 'Daycare Owner', 'Germany');

  -- ## YEAR
  INSERT INTO Year (year, user_id) VALUES
  (2023, 1),
  (2024, 2);

  -- ## EUBirthData
  INSERT INTO EUBirthData (eubd_id, country_code, birth_rate, crude_birth_rate, year) VALUES
  (1, 'BE', 10.8, 10.9, 2023),
  (2, 'DE', 9.3, 9.4, 2024);

  -- ## EUEmployment
  INSERT INTO EUEmployment (eue_id, year, country_code, workforce, self_employment, work_hours_weekly, sex, industry_sector) VALUES
  (1, 2023, 'BE', 29500000, 11.2, 36.5, 'Female', 'Transportation'),
  (2, 2024, 'DE', 44800000, 9.8, 35.2, 'Male', 'Finance');

  -- ## Children_FamilyBenefits
  INSERT INTO Children_FamilyBenefits (cfb_id, year, country_code, support_program, dependent_type, euro_amount) VALUES
  (1, 2023, 'BE', '$ for families', 'Child under 18', 1912.12),
  (2, 2024, 'DE', 'Alien Assistance', 'First and Second Child of Asylum Seekers', 25.00);

  -- ## PolicyAnalysis
  INSERT INTO PolicyAnalysis (analysis_id, user_id, country_code) VALUES
  (1, 1, 'BE'),
  (2, 2, 'DE');

  -- ## PolicyDetails
  INSERT INTO PolicyDetails (details_id, cost_per_month, policy_type, effect_on_birth_rate, analysis_id) VALUES
  (1, 450.00, 'Universal Childcare', 2.3, 1),
  (2, 320.00, 'Parental Leave', 1.8, 2);

  -- ## BusinessPlanning
  INSERT INTO BusinessPlanning (plan_id, daycare_id, year_forecast, user_id) VALUES
  (1, 101, 2026, 2),
  (2, 102, 2028, 2);

  -- ## GeneralLogistics
  INSERT INTO GeneralLogistics (oper_id, staffing_demand, financial_analysis, plan_id) VALUES
  (1, 12, 'Projected: €580,000/year. Staff: €380,000. Operating: 1.5%', 1),
  (2, 18, 'Expansion needs €250,000 investment.ROI: 22%', 2);

  -- ## OperatingHours
  INSERT INTO OperatingHours (hours_id, plan_id, year_forecast, daycare_id) VALUES
  (1, 1, 2025, 101),
  (2, 2, 2026, 102);

  -- ## ChildcareOptions
  INSERT INTO ChildcareOptions (option_id, country_code, cost_per_month, user_id) VALUES
  (1, 'BE', 650.00, 1),
  (2, 'DE', 450.00, 2);
</textarea>



# ML Proof of Concept