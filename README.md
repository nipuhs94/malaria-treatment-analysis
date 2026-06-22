# malaria-treatment-analysis
R Studio data analysis project exploring malaria treatment delays

Malaria Treatment Delay Analysis in Children Under Five

Project Overview

This project investigates factors contributing to delayed malaria treatment among children under the age of five across African countries. Malaria remains a major public health challenge, particularly in underdeveloped regions where limited healthcare access, medication availability, caregiver awareness, and infrastructure barriers can delay timely treatment.

The project uses survey data provided by The Kids Research Institute of Australia to analyse malaria treatment delays, identify key predictors, and visualise geographic patterns across Africa. The main aim is to support evidence-based public health decision-making by identifying regions and factors associated with delayed treatment.

Research Objective

The primary objective of this project is to develop a predictive model that can help identify children and regions at higher risk of delayed malaria treatment. The project also aims to create clear visualisations and spatial maps that communicate findings to non-technical stakeholders, such as public health teams, policy planners, and healthcare organisations.

Data Sources

The analysis was based on three survey datasets:

* Delay.csv
* Delay_covariates.csv
* Survey.csv

These datasets were merged using shared identifiers, including program, survey ID, region ID, district ID, cluster ID, respondent ID, and child ID. The final dataset was filtered to include African countries with valid geographic coordinates.

Methodology

The project followed a complete data analysis and modelling workflow in R:

Data Preparation

* Merged multiple survey datasets
* Cleaned missing and inconsistent values
* Converted empty values into missing values
* Filtered records to African countries
* Created a binary treatment delay outcome variable
* Recoded variables such as fever, cough, and health facility availability
* Converted categorical predictors into factor variables

Exploratory Data Analysis

* Analysed country-level malaria survey case counts
* Visualised cluster distributions across African countries
* Mapped survey points using geographic coordinates
* Compared delayed and non-delayed treatment cases
* Identified spatial patterns and high-delay regions
* Created animated temporal maps using gganimate

Modelling

Several statistical and machine learning models were developed and compared:

* Logistic Regression
* LASSO Regression
* Ridge Regression
* Linear Regression benchmark model
* Generalised Additive Mixed Model (GAMM)

These models were used to identify the strongest predictors of delayed malaria treatment and assess both individual-level and country-level variation.

Key Findings

Across the models, three predictors consistently emerged as the most important factors associated with delayed malaria treatment:

* Days taken to seek care
* Days taken to receive antimalarial treatment
* Health facility-related factors

The results suggest that treatment delays are more strongly influenced by healthcare accessibility and care-seeking timelines than by demographic factors such as wealth quintile, urban or rural status, or mother’s age.

The GAMM model captured nonlinear effects and country-level variation, showing that malaria treatment delays vary across national contexts and may be influenced by broader health system differences.

Visualisations

The project includes several visual outputs, including:

* Country-level malaria case count charts
* Cluster distribution charts
* Delay vs non-delay percentage charts
* Spatial maps of delayed treatment cases across Africa
* Cluster-level delay proportion maps
* Animated maps showing changes over time
* Regression coefficient plots

These visualisations were designed to make complex epidemiological and spatial findings easier to understand for non-technical stakeholders.

Technologies Used

* R
* RStudio
* R Markdown
* dplyr
* ggplot2
* sf
* leaflet
* rnaturalearth
* glmnet
* gamm4
* mgcv
* gganimate
* gifski
* caret
* pROC

Skills Demonstrated

* Data Cleaning
* Exploratory Data Analysis
* Spatial Data Analysis
* Statistical Modelling
* Predictive Analytics
* Logistic Regression
* Penalised Regression
* GAMM Modelling
* Data Visualisation
* Public Health Analytics
* Geospatial Mapping
* Research Reporting
* Stakeholder Communication

Project Outcome

This project demonstrates how data analytics and statistical modelling can support public health decision-making. By identifying predictors and geographic patterns of delayed malaria treatment, the analysis provides insights that could help guide targeted interventions, improve healthcare access, and support future malaria control strategies.

The project also provides a foundation for future spatially explicit modelling, such as Bayesian spatial modelling or INLA, to further improve the identification of high-risk regions and support evidence-based resource allocation.
