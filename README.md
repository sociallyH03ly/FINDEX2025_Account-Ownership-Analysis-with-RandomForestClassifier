# Account Ownership Analysis using Global Findex 2025 (Philippines) with Random Forest Classifier for Account Prediction 

## Project Overview
This analysis leverages metadata from the **Global Findex 2025 (Philippines)** to evaluate financial inclusion, specifically focusing on the factors that drive account ownership and the primary barriers keeping citizens unbanked.

### Key Findings
1. **Financial Inclusion Status:**
   * The baseline account ownership rate in the Philippines is **48.9%**, meaning over half of the adult population remains unbanked according to the survey sample.
   * Demographically, women comprise **56.6%** of the sample, while **38.0%** of respondents reside in urban areas.
   * The survey captures a wide age profile from 15 to 89 years, with a average (mean) age of 40.8 years and a median age of 40.5 years.

2. **Primary Barriers to Financial Inclusion:**
   * **Financial Constraints:** Out of the unbanked respondents, the most commonly cited barrier was **lack of money** to maintain or open an account.
   * **Cost & Distance:** Financial service fees and the physical distance to financial institutions represent major secondary bottlenecks.
   * **Lack of Documentation:** Many respondents report not having the necessary identification/paperwork required to open an account.

3. **Demographic Predictors (Model Insights):**
   * **Education** emerged as the strongest predictor of account ownership in our predictive pipeline.
   * **Urbanization** also plays a significant role, with urban residents having higher odds of being banked.
   * **Gender (Female)** had a minimal directly modeled correlation with account ownership on its own, showing that structural factors like education level and geographic region are much stronger drivers.

### Predictive Pipeline Performance
* **Model Accuracy:** Our models achieved **72.00% accuracy** on the test set, substantially outperforming the majority-class baseline of 51.50%.
* **ROC-AUC Score (0.743):** Indicates a good and stable discriminative capacity to classify banked vs. unbanked individuals based on basic demographic attributes.
* **Cohen's Kappa (0.440):** Suggests a fair-to-moderate agreement, validating that demographic variables hold robust predictive power.

### Strategic Recommendations
* **Policy Interventions:** Focus on bridging the education gap and enhancing financial literacy programs.
* **Digital ID Expansion:** Address the documentation barrier by continuing to scale national digital ID adoption.
* **Lower Entry Barriers:** Introduce zero-balance and low-fee accounts to mitigate the 'lack of money' and 'fee' constraints.
* **Expand Rural Digital Ecosystems:** Promote mobile money and digital banking agents in rural areas to bypass the physical distance barrier.
