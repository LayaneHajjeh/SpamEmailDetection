# Spam Email Detection Using Machine Learning
A Python-based machine learning project that uses Natural Language Processing (NLP) and supervised learning algorithms to classify emails as **Spam** or **Ham (Legitimate)**.
The project compares multiple machine learning models and evaluates their performance using different classification metrics and visualizations.

## Project Overview
Spam emails can contain malicious links, phishing attempts, and other security threats. Traditional rule-based filters can struggle when spammers change their techniques or modify suspicious words.
This project uses machine learning to automatically learn patterns from email messages and classify them as spam or legitimate.
The project was developed using Python in Google Colab.

## Dataset
* **Total messages:** 5,572
* **Spam messages:** 747
* **Ham messages:** 4,825
* **Spam:** 13.4%
* **Ham:** 86.6%
  
The dataset contains email message text and its corresponding label: `spam` or `ham`.

## Machine Learning Pipeline
The project follows the following workflow:
```text
Dataset
   ↓
Data Cleaning
   ↓
Text Preprocessing
   ↓
TF-IDF Feature Extraction
   ↓
Train / Test Split
   ↓
Machine Learning Models
   ↓
Model Evaluation
```


## Models Used
Three supervised classification models were trained and compared:
### Logistic Regression
A linear classification algorithm suitable for binary classification and large text datasets.

### Support Vector Machine 
A classification algorithm that works effectively with high-dimensional text features.

### XGBoost
An ensemble learning algorithm based on gradient boosting that was used to improve classification performance and handle the dataset effectively.

## Evaluation
The models were evaluated using several methods:
* Accuracy
* Confusion Matrix
* Classification Report
* ROC Curve
* Correlation Matrix
* Distance Matrix

The confusion matrix was used to analyze:
* True Positives — spam correctly identified
* False Positives — legitimate emails incorrectly classified as spam
* True Negatives — legitimate emails correctly identified
* False Negatives — spam emails missed by the model

## Results
The three models were trained using an **80% training and 20% testing split**.
Based on the evaluation results, **XGBoost achieved the best overall performance** among the tested models, including higher accuracy and spam recall.
The ROC curve and confusion matrices were also used to compare how effectively the models separated spam emails from legitimate emails.

## Technologies Used
* Python
* Google Colab
* pandas
* NumPy
* spaCy
* scikit-learn
* XGBoost
* Matplotlib
* Seaborn
* TF-IDF


## Project Purpose
This project demonstrates the application of machine learning and NLP techniques to a cybersecurity problem. It combines text preprocessing, feature engineering, supervised classification, and model evaluation to build and compare spam email detection models.
The results demonstrate how machine learning can be used to identify suspicious email messages and help improve automated email security.
