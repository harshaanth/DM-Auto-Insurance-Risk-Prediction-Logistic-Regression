# Auto Insurance Risk Prediction

This project aims to predict the risk of insurance claims based on various customer and vehicle factors. The analysis uses logistic regression to model the probability of a claim, helping an insurance company evaluate the risk associated with new contracts.

## Project Overview

An analyst at an insurance company noticed an increase in accident claims and decided to analyze the key factors that lead to claims. The goal is to develop a model using historical data to predict the risk of claims for new contracts based on the profile of the subscriber and the car insured.

## Methodology

1. **Data Preparation**: 
   - Categorical variables were transformed into dummy variables.
   - The data was split into training and validation datasets.
   - Stepwise variable selection was used to recommend models.

2. **Model Selection**:
   - The final logistic regression model selected is as follows:
   

Here is the README.md content formatted for direct use in your GitHub repository:

markdown
Copy code
# Auto Insurance Risk Prediction

This project aims to predict the risk of insurance claims based on various customer and vehicle factors. The analysis uses logistic regression to model the probability of a claim, helping an insurance company evaluate the risk associated with new contracts.

## Project Overview

An analyst at an insurance company noticed an increase in accident claims and decided to analyze the key factors that lead to claims. The goal is to develop a model using historical data to predict the risk of claims for new contracts based on the profile of the subscriber and the car insured.

## Methodology

1. **Data Preparation**: 
   - Categorical variables were transformed into dummy variables.
   - The data was split into training and validation datasets.
   - Stepwise variable selection was used to recommend models.

2. **Model Selection**:
   - The final logistic regression model selected is as follows:
   
**Logit (claim=1) = -1.65 -0.79 * woman -0.66 * children1 -0.62 * children2 -1.14 * childrenmorethan4 -0.63 * SUV + 0.44 * sport + 0.46 * diesel**


3. **Interpreting the Coefficients**:
- **Gender**: Women are 0.46 times less likely to make a claim than men.
- **Children**:
  - Customers with 1 child are 0.52 times less likely to claim.
  - Customers with 2 children are 0.54 times less likely to claim.
  - Customers with 4 or more children are 0.32 times less likely to claim.
- **Car Type**:
  - SUV owners are 0.53 times less likely to claim than sedan owners.
  - Sports car owners are 1.56 times more likely to claim.
- **Fuel Type**: Diesel car owners are 1.58 times more likely to claim than petrol car owners.

4. **Customer Profile Most Likely to Claim**:
- Male
- No children or 3 children
- Sports car owner
- Diesel fuel

5. **Odds of Claiming**:
- For example, the odds that a man with one child and a petrol sedan would claim are calculated using the model. The result shows that the probability of this man making a claim is below the cutoff value of 0.5, meaning he would not be classified as likely to claim.

## Repository Contents

- `README.md`: This file, providing an overview of the project.
- `HW_4_Project_Report.pdf`: Detailed project report with analysis and results.
- `HW_4_Auto_Insurance_Risk.xlsx`: The dataset used for analysis.
