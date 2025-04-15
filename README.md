# Lead Conversion Model for X Education

## Overview
X Education, an online course provider, seeks to improve lead conversion efficiency by identifying high-potential leads. This project builds a logistic regression model to score leads based on conversion probability, enabling optimized sales efforts.

## Objective
- Improve the lead conversion rate from ~30% to ~80%
- Develop a predictive model to classify leads as high or low probability of conversion
- Provide actionable insights to improve sales strategies

## Data Preprocessing
- Handled missing values by imputation or removal
- Encoded categorical variables using dummy variables
- Treated "Select" category as null values
- Scaled numerical features for better model performance

## Model Development
- Logistic Regression model chosen for its interpretability and suitability for binary classification
- Feature selection using Recursive Feature Elimination (RFE)
- Model trained using a 70:30 train-test split
- Evaluated using accuracy, precision, recall, and F1-score

## Key Findings
### Top Influencing Variables
- `Tags_Lost to EINS`
- `Tags_Closed by Horizzon`
- `Tags_Will revert after reading the email`

### Key Categorical Variables
- `Lead Source`: Where the lead originated
- `Last Activity`: Most recent engagement of the lead
- `Specialization`: Industry of the lead

### Model Performance
- Achieved ~80% accuracy on test data
- Balanced precision and recall to minimize false negatives

## Business Recommendations
### **Peak Hiring Period (Intern Hiring Phase)**
- Lower probability threshold (e.g., 0.4 instead of 0.5) to capture more leads
- Increase follow-ups with interested but non-responsive leads
- Prioritize leads tagged as "Will revert after reading the email"

### **Quarterly Target Achieved Early**
- Raise probability threshold (e.g., 0.7 or 0.8) to focus only on high-potential leads
- Prioritize highly engaged leads with strong intent signals (e.g., requested course details)
- Reduce phone calls for low-engagement leads and rely on email/SMS outreach

## Conclusion
The logistic regression model enables data-driven lead scoring, helping X Education optimize resource allocation. Implementing strategic adjustments based on business needs will further enhance lead conversion rates and sales efficiency.
