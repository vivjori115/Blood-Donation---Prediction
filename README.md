# Blood Donation - Prediction

This project aims to develop a predictive model for blood donation behavior using Logistic Regression. The dataset consists of features such as recency, frequency, monetary value, and time since the first donation. The objective is to forecast whether a donor will give blood during the next visit of the donation vehicle to a university campus.

## Overview

The notebook employs the following libraries:
- pandas
- numpy
- seaborn, matplotlib
- sklearn

## Exploratory Data Analysis (EDA)

EDA focuses on understanding the underlying patterns and relationships within the dataset. Key insights include:

- **Donation Frequency Distribution**: The histogram reveals a skewed distribution of blood donation frequency among donors. Most donors have made relatively few donations, indicating potential opportunities for encouraging repeat donations.

- **Recency vs. Frequency Relationship**: The scatter plot illustrates a clustering of points indicating that a majority of donors have made relatively recent donations. This suggests that donors are more likely to donate blood again within a relatively short time frame.

- **Time Since First Donation vs. Blood Donation Volume**: The scatter plot demonstrates that donors who have been engaged in blood donation for a longer duration tend to contribute a larger volume of blood. This indicates a sense of commitment and loyalty to the cause over time.

## Model Selection

The notebook utilizes TPOT (Tree-based Pipeline Optimization Tool) for automated model selection. TPOT searches through various machine learning pipelines to find the optimal one for the dataset. The selected model is then further optimized and evaluated using the Area Under the Curve (AUC) score.

## Conclusion

In conclusion, the project explores the significance of features such as time, frequency, recency, and monetary value was highlighted in predicting blood donation. Exploratory Data Analysis (EDA) uncovered insights into distribution of blood donation, relationships between donation recency and frequency, and between first time donation and volume of blood donated.

TPOT was utilized for automatic model selection, achieving an AUC score of 0.785. Furthermore, log normalization of the training data resulted in a 0.5% improvement in AUC score.

This model can be utilized by blood donation centers to optimize donor outreach and retention strategies, ultimately ensuring a stable blood supply to save lives.
