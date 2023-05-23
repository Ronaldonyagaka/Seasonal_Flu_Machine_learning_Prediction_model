# Seasonal Flu Machine learning Prediction_model
A prediction Model of Season Flu Vaccine uptake

![seasonal](https://wwwassets.rand.org/content/rand/pubs/research_briefs/RB9572/jcr:content/par/teaser.fit.0x1200.jpeg/1495291580551.jpeg)
## Introduction
The occurrence of the flu season repeats annually, and each year people make a choice to either receive the flu shot or not.

This attempts to develop a predictive model to forecast individuals' decision to receive the flu shot or not during the annual flu season.

The model should leverage historical data to identify patterns and factors that influence people's vaccination choices.

By analyzing variables such as age groups, genders, and other relevant characteristics, the goal is to accurately predict whether an individual will opt for the flu shot or not.

This predictive model aims to assist in public health planning and decision-making by providing insights into vaccination trends and helping allocate resources effectively to the United States government health Agencies

## Main Objectives
- Investigate factors influencing individuals' decision to receive the flu shot during the annual flu season, excluding any explicit goals.
- Analyze variables such as age groups, genders, and presence of children in households to understand their statistical implications.
- Address inquiries related to targeting specific subsets of the population to enhance the overall vaccination rate.
- Build a predictive model to determine whether or not given certain features or conditions, people would receive the Seasonal Flu Vaccine

## Data Description
The datasets used for this project were downloaded from Kaggle. 
It contains information on the social,economic and demographic backgrounds of the respondents as well as their opinions on the H1N1 and seasonal flu vaccines. 
The training data has 26707 rows and 36 columns

## Data Preparation
After loading the data, it was evaluated, and exploratory data analysis (EDA) was conducted to gain a deeper understanding of the dataset. 
During this process, it was observed that there were numerous missing values, which were addressed by replacing them with appropriate values. 
Since all the features in the dataset are categorical, their data types were modified to facilitate ordinal encoding. 
This transformation was necessary to prepare the data for modeling purposes.

## Modelling
The data was split into the training and test datasets . The baseline model was created using Decision Tree. 
RandomForest GradientBoostingClassifier, ADABoosting, XGBoosting and CATBoosting were used

## Model Evaluation
The model selection was based on the following criteria:

- Accuracy and ability to generalize over unseen data.
- Time taken to process data and make a prediction.
- Potential to learn from more data and not be at risk of over-fitting.

## Conclusion
The data set was biased towards certain communities and classes.
This makes the models generated biased towards this group of people and may not reflect the general situation.
The gradient boosting model was optimal despite existing biases within our features.

## Recommendations

- Communication of limitations, biases, and specific applicability of the models, along with comprehensive documentation should be adhered to.

- Techniques such as oversampling, undersampling, or the utilization of weighted loss functions can be employed to mitigate biase.

- Careful examination of the significance of identified predictors, such as opinion_seas_risk, will help understand underlying factors and ensure fairness in decision-making

- Validate conclusions by incorporating external data from various sources

- Include a wider range of demographic groups, thereby achieving a more diverse and balanced dataset.
