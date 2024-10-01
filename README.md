# Beer Type Predictor Based on ABV and IBU

## Project Overview

This project applies **machine learning** techniques to predict the type of beer based on its characteristics, specifically **Alcohol By Volume (ABV)** and **International Bitterness Units (IBU)**. Using a publicly-available dataset on craft beers from Kaggle, I implemented a classification model to predict the beer style from its ABV and IBU values, focusing on the four most common beer styles: 

- American IPA
- American Pale Ale (APA)
- American Amber / Red Ale
- American Double / Imperial IPA

This project showcases my ability to handle real-world datasets, preprocess data, and build predictive models using **scikit-learn** and other Python libraries.

## Dataset

The dataset used for this project is sourced from Kaggle and contains detailed information on over 2,000 beers brewed by 500+ breweries. Features such as **ABV**, **IBU**, and beer styles were utilized in building the model.

- **Beer Dataset**: Contains beer-specific information like name, style, ABV, and IBU.
- **Breweries Dataset**: Contains information about the breweries that produce these beers.

The two datasets were merged and preprocessed to remove missing values and retain only relevant beer characteristics.

## Machine Learning Model

A **Support Vector Machine (SVM)** classifier with a linear kernel was used to predict the beer type. The model was trained using 80% of the dataset, with the remaining 20% used for testing. Key steps in the model development include:

- **Data Preprocessing**: Handled missing values, merged datasets, and scaled features where necessary.
- **Feature Selection**: The model was trained using ABV and IBU as predictors, while beer style was the target variable.
- **Model Training**: A linear SVM classifier was chosen due to its performance in high-dimensional spaces and effectiveness in multi-class classification tasks.
- **Model Evaluation**: Performance metrics like **precision**, **recall**, **F1-score**, and **confusion matrices** were used to assess the model’s predictions.

## Key Results

- Achieved an overall accuracy of **66%** on the test set, with precision and recall varying across beer styles.
- The model performed best when predicting **American IPA** (72% recall on test data) and struggled with **American Double / Imperial IPA**, likely due to overlap in characteristics with other styles.
- Confusion matrices and classification reports were generated to analyze misclassifications and optimize the model further.

## Skills Demonstrated

- **Data Wrangling**: Merged datasets, handled missing data, and prepared data for machine learning.
- **Machine Learning**: Applied an SVM classifier and evaluated the model using key metrics.
- **Python Libraries**: Utilized **pandas**, **NumPy**, and **scikit-learn** for data manipulation and model building.
- **Model Evaluation**: Analyzed model performance through confusion matrices and classification reports.
