## Project: Modeling Smoking Behavior in Bangladesh: Logistic Regression with Random Effects Analysis  

# Overview
This project investigates the factors influencing smoking behavior among adults in Bangladesh. Using logistic regression and random effects modeling, the study aims to identify the socio-demographic and environmental factors associated with smoking, with a specific focus on the use of a dataset from the Global Adult Tobacco Survey (GATS) - Bangladesh 2017.  

# Project Objective  

The primary goal of this analysis is to:  
- Identify the socio-economic, demographic, and environmental factors influencing smoking behavior.  
- Understand the impact of variables such as gender, education, and wealth index on smoking.  
- Incorporate random effects to account for data clustering within geographical divisions.

# Dataset

The dataset used for this analysis is the **Global Adult Tobacco Survey (GATS) - Bangladesh 2017**, consisting of 12,783 respondents. After cleaning, down-sampling, and feature engineering, the final dataset includes key socio-demographic variables such as:
- Age
- Gender
- Wealth index
- Education level
- Region/division
- Residence (urban/rural)
- Access to schools, hospitals, and restaurants

# Methodology

## 1. Data Preparation

- Data cleaning and handling of missing values were performed.
- Feature engineering was applied to create variables such as wealth index and access to resources (schools, hospitals, etc.).
- Data was grouped by regions (geographical divisions) to account for potential clustering.

## 2. Statistical Modeling
- Logistic Regression: The primary model used was logistic regression due to the binary nature of the dependent variable (smoking status: smoker vs. non-smoker).  
- Random Effects: A generalized linear mixed model (GLMM) was used to account for random effects due to clustering in the data by geographical divisions.  
- Model Validation: Model performance was evaluated using metrics such as AIC, residual plots, and marginal effects.  
## 3. Results
- Gender and education level were found to be significant predictors of smoking behavior.  
- Geographic disparities were also observed, with regions like Dhaka and Mymensingh showing a higher prevalence of smoking.  
- The wealth index and other factors such as access to hospitals, transport, and schools did not have significant effects on smoking behavior.  
## Conclusion
This study highlights key determinants of smoking behavior among adults in Bangladesh, emphasizing the role of gender, education, and geographical division. These findings suggest that targeted interventions are necessary to address the smoking epidemic in specific demographics and regions.  
## Requirements
To run this analysis, the following R libraries are required:  

- dplyr  
- readxl  
- psych  
- lme4  
- DHARMa  
- survey  
- margins

Install the required packages in R using:  

```
install.packages(c("dplyr", "readxl", "psych", "lme4", "DHARMa", "survey", "margins"))
```
## Running the Analysis  
1. Load the dataset and necessary libraries.  
2. Perform data cleaning and feature engineering.  
3. Run logistic regression and GLMM models using the code provided.  
4. Validate the model using residual analysis and AIC.  
5. Interpret the results based on the model summary.  

  

 
