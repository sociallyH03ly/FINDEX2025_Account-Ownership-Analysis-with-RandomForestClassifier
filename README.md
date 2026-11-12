# Account-Ownership-Prediction-using-RandomForestClassifier
## Overview
 This machine learning project uses 2024 Global Findex - Philippines Microdata, containing 1,000 cases (survey responses) and 199 variables. The dataset was cleaned and preprocessed using python techniques. After cleaning, investigating, and preprocessing, the dataset was used to turn into a modeled prediction of account ownership with a Random Forest Classifier using synthesized individual-level microdata. The trained model yielded a 70.50% test set accuracy and identified education level as the most important predictor.

 ## Result during the analysis
 1. Loaded the JSON File: We parsed /content/Findex/PHL_2024_FINDEX_v02_M.json successfully by handling its nested metadata dictionary structure.
 2. Extracted Key Structures: We converted the file descriptions (df_files) and the extensive variable metadata (df_vars) into separate Pandas DataFrames.
 3. Analyzed Distributions: We plotted the distribution for the female variable, showing a sample size of 566 females and 434 males out of the 1,000 respondents in the Philippines survey.
 4. Recovered Variable Labels: Found that the variable descriptions were stored in labl (rather than the empty var_txt field) and cleaned the dataset with descriptive names.
 5. Analyzed Core Demographics: Plotted the distribution of female (female) and education (educ) levels in the survey.
 6. Ranked Reported Challenges: Identified that securing emergency funds (63.8% very difficult) and financial institution barrier variables (like lack of money at 46.9% and fees too expensive at 35.6%) were the most frequent challenges reported in the dataset.
 7. Emergency Funds: 63.8% of the 1,000 respondents find securing emergency funds "Very difficult".
 8. Education Level: The sample is composed of 38.0% with Primary education or less, 54.2% with Secondary education, and 7.8% with Tertiary education or more.
 9. Urbanicity shows a split of 620 Rural (62.0%) vs. 380 Urban (38.0%).
 10. Account displays a nearly even split of 511 without an account (51.1%) vs. 489 with an account (48.9%).

## Machine Learning Demonstration Results
1. Predictive Performance:
 - Overall Accuracy: 70.50% on the hold-out test set (200 respondents).
 - For Account Holders (Has Account): The model achieved a recall of 94% and precision of 72%, indicating it is highly capable of identifying those who own financial accounts.
 - For Non-Account Holders (No Account): The model had lower recall (19%), which is typical when training on highly structured discrete synthetic probabilities.
2. Feature Importances:
 - Education Level (education): ~54.8% importance (By far the strongest predictor, matching our synthesis logic that higher education increases access).
 - Urbanicity (urban): ~27.0% importance.
 - Gender (female): ~18.2% importance.

