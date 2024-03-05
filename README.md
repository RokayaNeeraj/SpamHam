# NLP Spam Detection Project Summary

This Jupyter Notebook automates the process of building a Support Vector Machine (SVM) model for spam email detection.

## Functionality:

### Data Loading and Preprocessing:

- Loads email data from separate folders for ham and spam emails.
- Performs text cleaning using regular expressions.
- Extracts features like date count, non-URL word count, emoji count, etc.
- Calculates email length, capital letter count, and ratios.
- Identifies the presence of common spam phrases and suspicious keywords.
- Checks for personalization and unsubscribe links.

### Feature Engineering:

- Applies tokenization to split text into individual words.
- Handles missing values.
- Creates a Bag-of-Words (BoW) representation using CountVectorizer.
- Scales features using StandardScaler.

### Model Building and Evaluation:

- Splits data into training and testing sets.
- Trains a linear SVM model with balanced class weights.
- Performs 5-fold stratified cross-validation to evaluate model performance.
- Calculates and reports various metrics, including accuracy, precision, recall, F1-score, and AUC-ROC.
- Visualizes the ROC curve and confusion matrix.

## Key Points:

- AUC Score: The model achieves an average AUC score of 0.98 across folds, indicating good discrimination between spam and ham emails.
- Feature Importance: Features like email length, capital letter count, URL count, and presence of spam phrases seem to play a significant role in spam detection.
- Further Exploration: Explore other feature engineering techniques, different machine learning algorithms, and hyperparameter tuning for potential performance improvements.

## Getting Started:

- Clone or download this repository.
- Install required libraries: pandas, numpy, os, re, scikit-learn, seaborn, matplotlib, gensim.
- Execute the Jupyter Notebook.

## Note:

- This is a basic example and may require adjustments for specific datasets and requirements.
- Consider incorporating domain knowledge and ethical considerations when building spam detection models.
