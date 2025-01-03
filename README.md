# NoSQL Challenge: Food Hygiene Database Analysis

##  Overview

This challenge involves analyzing food hygiene ratings data provided by the UK Food Standards Agency. The goal is to assist the editors of the food magazine **Eat Safe, Love** in identifying key insights from the database, which will help them determine focus areas for future articles.

The challenge is implemented using MongoDB for database operations and Python (Jupyter Notebooks) for data manipulation and exploratory analysis.

## Objectives

1. **Database Setup**  
   - Import data from the `establishments.json` file into a MongoDB database named `uk_food`.
   - Validate database setup and perform initial checks on the data.

2. **Database Updates**  
   - Insert new establishment data (e.g., "Penang Flavours" restaurant).
   - Update and clean data, including converting string values to appropriate data types.
   - Remove irrelevant data (e.g., establishments in Dover).

3. **Exploratory Data Analysis**  
   - Identify establishments with specific characteristics (e.g., hygiene score, rating).
   - Perform geographic queries to find establishments near a specific location.
   - Aggregate data to identify patterns and trends.

## Files

### Starter Files
- `NoSQL_setup_starter.ipynb`: Jupyter Notebook for database setup and updates.
- `NoSQL_analysis_starter.ipynb`: Jupyter Notebook for exploratory data analysis.
- `establishments.json`: JSON file containing the dataset.

### Additional Files
- `README.md`: Project documentation (this file).
## Steps to Reproduce

### 1. Database and Jupyter Notebook Setup
- Import the data using the following MongoDB command:
  ```bash
  mongoimport --db uk_food --collection establishments --drop --file establishments.json

## Observations and Insights
1.Poor Hygiene Score Establishments:A significant number of establishments (41) have the worst possible hygiene score of 20.
2.Good Hygiene Establishments in London:33 establishments in London have a RatingValue ≥ 4, showing better hygiene standards compared to the first group.
