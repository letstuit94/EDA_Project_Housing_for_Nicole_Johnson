# 1. Overview and Objectives

## Background

In this project, we analyze the King County housing dataset, which contains information on real estate sales in the Seattle area. The goal is to identify patterns, trends, and relationships in the housing market using Exploratory Data Analysis (EDA) and statistical methods.

The analysis will be conducted using SQL and Python, combining database querying with deeper analytical insights.

## Objective of the Analysis

The main objective is to generate data-driven insights that support informed decision-making for a potential home buyer. The analysis is tailored to a specific persona:

**Nicole Johnson**
- Buyer
- Looking for a lively, central neighborhood
- Mid-range budget
- Purchase timeline: within one year

## Key Questions

The analysis aims to answer the following questions:
- Which factors have the strongest impact on housing prices?
- Which neighborhoods offer the best value for money?
- How do central and suburban locations differ in terms of price and quality?
- Are there seasonal trends or optimal times to buy?

## Expected Outcomes

Throughout the analysis, we aim to:
- Identify at least 3 data-driven insights (including one geographical insight)
- Develop at least 3 actionable recommendations for Nicole

## Value for the Persona
The findings will help Nicole to:
- Identify suitable neighborhoods
- Optimize her budget allocation
- Choose the right timing for purchasing a property

# 2. Data Description

## Dataset Overview

The dataset used in this analysis is the King County Housing Dataset, which contains information on residential property sales in King County, Washington (including Seattle) between May 2014 and May 2015.
Each row in the dataset represents a single property sale, with detailed information about the property’s characteristics, location, and sale price.

## Key Features (Columns)

The dataset includes a mix of numerical and categorical variables. The most relevant features for our analysis are:

- **price**: Sale price of the house (target variable)
- **bedrooms**: Number of bedrooms
- **bathrooms**: Number of bathrooms
- **sqft_living**: Living area size (in square feet)
- **sqft_lot**: Lot size (in square feet)
- **floors**: Number of floors
- **waterfront**: Whether the property has a waterfront view (0 = no, 1 = yes)
- **view**: Quality of the view (ordinal scale: )
- **condition**: Overall condition of the house
- **grade**: Construction and design quality
- **sqft_above**: Square footage above ground
- **sqft_basement**: Square footage of basement
- **yr_built**: Year the house was built
- **yr_renovated**: Year of last renovation (if applicable)
- **sqft_living15**: Average living space of the 15 nearest neighboring houses
- **sqft_lot15**: Average lot size of the 15 nearest neighboring houses
- **zipcode**: ZIP code of the property
- **lat / long**: Geographic coordinates
- **date**: Date of sale

## Data Structure

- **Number of observations**: around 21600 properties
- **Number of features**: 21 variables
- **Data types**:
  - Numerical: e.g., price, sqft_living, bedrooms
  - Categorical/ordinal: e.g., condition, grade, view
  - Temporal: e. g., date of sale
  - Geospatial: e. g., zipcode, latitude and longitude

## Initial Observations

- The dataset includes both property-specific features (size, condition) and location-based features (zipcode, lat/long).
- The price variable shows high variability, indicating a diverse housing market.
- Geographic data (lat/long, zipcode) will be especially important for identifying location-based insights, which are key for the persona.

## Relevance for the Analysis

This dataset is well-suited to:
- Analyze price drivers (e.g., size, quality, location)
- Identify trends over time
- Support data-driven recommendations for a buyer like Nicole