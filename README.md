# Exploratory Data Analysis (EDA) for Real Estate Pricing

## Project Overview

This project explores the factors that influence house prices in the residential real estate market. Using the provided dataset, we perform an in-depth **Exploratory Data Analysis (EDA)** to uncover patterns, trends, and relationships among different variables that affect house prices. By analyzing the dataset through visualizations, correlations, and statistical analysis, we aim to guide better decision-making in pricing strategies, property acquisition, and sales for a real estate company.

### Problem Statement:
The real estate market is complex, with numerous factors influencing the pricing of residential properties. Through this project, we aim to:
- Identify key variables that impact house prices.
- Explore relationships between different features like house size, age, amenities, and location.
- Provide actionable insights to help inform pricing strategies for better business outcomes.

## Dataset

The dataset used in this project is a housing data set that contains information about residential properties. The dataset has 1460 rows and 81 columns, with various features related to house characteristics, amenities, and historical sales.

### Key Columns:
- **SalePrice**: The target variable (house price).
- **OverallQual**: Overall quality of the house (an integer scale).
- **GrLivArea**: Above ground living area in square feet.
- **YearBuilt**: Year the house was built.
- **LotArea**: Lot size in square feet.
- **Neighborhood**: The neighborhood where the house is located.
- **BldgType**: Type of the building (e.g., single-family, duplex).
- **GarageCars**: Number of cars that can fit in the garage.

### Data Source:
- The data used in this project is https://drive.google.com/file/d/1QArG-18iCogBSk-_06998eUhfb9YLZPa/view

## Project Structure

The project is organized as follows:
Real-Estate-Analysis/
│
├── data/
│   └── Housing Data.csv        # The dataset used in the analysis.
│
├── code/
│   └── EDA_Real_Estate.ipynb   # Jupyter notebook with all the code.
│
└── README.md                   # This file.

## Setup Instructions

1. **Clone the repository**:
    ```bash
    git clone (https://github.com/abhisharudra/My-project-3.git)
    cd Real-Estate-Pricing-EDA
    ```

2. **Install dependencies**:
    - Create a virtual environment and install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```
    - Required libraries include:
      - `pandas`
      - `numpy`
      - `matplotlib`
      - `seaborn`
      - `jupyter`

3. **Run the Jupyter notebook**:
    - Launch Jupyter Notebook to start the analysis:
    ```bash
    jupyter notebook
    ```
    - Open the notebook `Abhishek_project_3.ipynb` and execute the cells to reproduce the analysis and results.

## Key Steps in the Analysis

1. **Data Loading & Cleaning**:
    - Load the dataset into a Pandas DataFrame.
    - Handle missing values, remove duplicates, and address anomalies.
  
2. **Univariate Analysis**:
    - Explore the distribution of individual variables such as house prices, size, and overall quality.
    - Visualize distributions using histograms, boxplots.

3. **Multivariate Analysis**:
    - Investigate relationships between multiple variables, especially features impacting house prices.
    - Compute and visualize correlation matrices and scatter plots to uncover patterns.

4. **Feature Engineering**:
    - Create new features such as *price per square foot* and *property age*.
    - Evaluate how different features impact house prices through scatter plots and regression analysis.

5. **Insights & Conclusions**:
    - Identify key variables like `OverallQual`, `GrLivArea`, and `YearBuilt` that have the highest impact on house prices.
    - Explore how external factors such as `Neighborhood` and amenities (e.g., swimming pool, garage) influence house valuations.

6. **Visualizations**:
    - Generate and save key visualizations like correlation heatmaps, histograms, and scatter plots.

## Key Findings
- The **Age of the Property** (`YearBuilt`) also impacts prices, with newer homes generally having higher prices.
- **Amenities** such as swimming pools and garages significantly increase property prices.
- Market trends indicate an upward price trend over the years, with some fluctuations based on external factors like economic conditions and neighborhood desirability.

## Challenges Faced

- **Missing Data**: Some columns like `Alley` had a lot of missing values, which were handled by imputing or dropping them.
- **Outliers**: Some extreme values in the `SalePrice` column were considered, but outliers were handled by investigating their impact on the results.
- **Categorical Data**: Several categorical columns needed encoding before being used in modeling or further analysis.

## Next Steps

- Feature selection and dimensionality reduction to prepare for predictive modeling.
- Building predictive models such as linear regression, decision trees, or XGBoost to predict house prices based on the EDA findings.
- Further analysis on categorical features using techniques like one-hot encoding or label encoding



