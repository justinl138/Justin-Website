
<div align="center">
  <h1>Predicting Patient Outcomes (Proprietary)</h1>
</div>

## Tools and Concepts Applied
1. R
2. Tidyverse packages - dplyr, ggplot
3. Pearson's correlation coefficient
4. Correlation Matirx
5. General Linearized Models - Logistic Regression 


## Introduction

My team at Edwards Lifesciences wanted to utilize patient measurements to predict whether a mitral/tricuspid repair procedure would pose procedural risks: lengthy procedure time and insufficient reduction in regurgitation. 

## Data

I was given 3 separate patient datasets from the CLASP 2TR Clinical Trials.

The goal of the CLASP II TR clinical trial is to determine the safety and effectiveness of the Edwards PASCAL transcatheter valve repair system. This study targeted patients with symptomatic severe tricuspid regurgitation during preliminary screening.

The datasets contained 150+ parameters taken from 300+ patients. Features included physiological measurements, ID#’s, and timestamps. The rows represented patients (each patient had a unique ID#) and the columns represented features that were both continuous and categorical in nature.



## Data Processing

Data Transformation:
The 3 data sets were merged by unique patient ID’s. New features were engineered from preexisting features. For example, durations were calculated with timestamps. Labels that marked each patient as having a “long procedure time” or “insufficient reduction” were assigned based off a set criteria. Mean imputation was used to fill in missing values.

Data Reduction:
Patients that did not fit certain criteria, such as undergoing a complete procedure, were removed. Pearson correlation coefficients between independent features were analyzed and visualized with a correlation matrix. When independent features were highly correlated, we only retained one of these features. 



## Exploratory Modeling 
We fit logistic regressions to various categorical and predictor variables. By observing various log-odds coefficients, we distinguished which predictor variables had the largest impact on the likelihood of a certain risk being observed. 


## Results and Next Steps
Successfully narrowed down to 3 uncorrelated features that had a significant impact on the likelihoods of lengthy procedure time and insufficient reduction. 

Next Steps: 
1. Exploring logistic regressions with multiple predictor variables.
2. Creating the binary classification models and evaluating the performance of our models by partitioning our dataset into testing and training data set


