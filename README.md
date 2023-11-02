# Project Title: YouTube Trending Video Analysis

## Overview

The aim of the project is to predict the view count of YouTube videos using various features such as likes,dislikes,view count,comment count and other relevant metadata. The project involves data preprocessing, feature engineering, exploratory data analysis (EDA), model selection and training, model evaluation,  final prediction, and interpretation. By following these steps, the project seeks to provide insights into the factors that influence a video's view count and to develop a model that can accurately predict the number of views a video is likely to receive.

The project will help answer the following questions:

### Question 1

What are the key factors influencing the view count of YouTube videos?

### Question 2

How do different metadata features, such as video title, tags, and description, correlate with the view count?

### Question 3

What are the most significant features that contribute to the prediction of view count, and how do they influence the outcome?

### Question 4

Which machine learning model performs the best in predicting the view count of YouTube videos based on the available data?
  
### Question 5

How reliable is the developed model in making predictions about the view count of new YouTube videos?

By addressing these questions, the project can provide valuable insights for the view counts that can be expected after the video is published in long run and the chances of achieving higher view counts.

## Source of Data

The dataset was obtained from Kaggle.

## Findings

### Question 1/ Answer

View count was found to depend on : likes, comment count, tag , category and title.

### Question 2/Answer

The specific words in video titles impact the view counts.
The titles Words like official and trailer in titles.
Similarly, specific tags like officil or trailer wereshown to give high views count.

### Question 4/Answer

Random Forest is the best model.

### Question 5/Answer

Random Forest Regressor and Decision Tree Regressor models exhibited perfect performance, as indicated by a mean squared error of 0.00 and a coefficient of determination of 1.00

But, because Random Forest is an ensemble model built on multiple decision trees, it reduces overfitting and improves generalization. For this reason, Random Forest is used as the best model.

## Dependencies
Requirements and requirements dev file for reference :
https://github.com/MeghaBhambri/youtube_engagement_analysis/blob/main/requirements-dev.txt

https://github.com/MeghaBhambri/youtube_engagement_analysis/blob/main/requirements.txt

## Installation

- Clone the repository or download the project files.
- Ensure the necessary dependencies are installed.


## Instructions

- Install the required dependencies using pip or any other package manager.
- Ensure the 'US_youtube_trending_data.csv' and 'US_category_id.json' files are in the correct data directory.
- Adjust file paths if necessary before running the script.

## Scripts

### 1. Understanding and preprocessing data(notebooks/understanding_preprocessing_data.ipynb)

- understanding data
- cleaning data 
- checking info/nans/changing column names

### 4. Visualization(notebooks/exploratory_analysis.ipynb)

- Visualize null values by column using a bar plot created with Seaborn.
- Generate a heatmap to display correlations between specific columns.
- Create bar plots to demonstrate category-wise view counts.

### 5. Machine Learning Analysis(notebooks/feature_analysis_model_creation.ipynb)

- Preprocess data for machine learning models, including label encoding and data transformation.
- Train various regression models, including Linear Regression, Random Forest Regressor, Decision Tree Regressor, and K-Nearest Neighbors Regressor.
- Perform model evaluation and predictions for view count.

## Prediction Functionality

The project also offers an interactive Gradio interface for predicting the view count of a video for a specified time period. The trained machine learning model can be utilized for this purpose.

## Conclusion

Based on the findings from the analysis, the project concludes that various factors, including likes, comment count, video tags, and specific words in the title, significantly influence the view count of YouTube videos. Moreover, the analysis revealed that the Random Forest Regressor is the best-performing model for predicting YouTube video view counts, considering its robustness and generalizability. Despite the Decision Tree Regressor also exhibiting perfect performance, the ensemble nature of the Random Forest Regressor makes it a more suitable choice for this particular project.

## Next Steps

In the next steps, further enhancements can be made to the data preprocessing pipeline, including additional feature engineering to extract more meaningful insights from the video metadata. Additionally, the project could benefit from an expanded dataset to improve the robustness and accuracy of the predictive models. Regular updates and retraining of the machine learning models based on the latest data would also contribute to more accurate predictions.

## Contributors

- [Megha](https://github.com/MeghaBhambri)

Feel free to contribute or provide feedback on the project. Thank you for using our YouTube Trending Video Analysis tool!
