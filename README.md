Customer Complaint Classification using NLP & Topic Modeling
Overview

This project builds an automated customer complaint classification system for a financial services company. The goal is to categorize customer complaints into relevant product/service groups using Natural Language Processing (NLP), Topic Modeling, and Machine Learning.

The project first uses Non-Negative Matrix Factorization (NMF) to discover hidden complaint topics from unlabeled customer complaints. These discovered topics are then mapped to business categories and used to train supervised machine learning models for automatic complaint classification.

Business Problem

Financial institutions receive thousands of customer complaints related to products and services such as:

- Credit Cards
- Bank Accounts
- Mortgages & Loans
- Fraud & Dispute Reporting
- Other Financial Services

Manually routing these complaints to the appropriate department is time-consuming and inefficient. This project automates the categorization process to improve response time and customer satisfaction.

Dataset
- Format: JSON
- Records: 78,313 customer complaints
- Features: 22 columns
- Source: Consumer Financial Protection Bureau (CFPB) complaint dataset
- Project Workflow
1. Data Loading
- Loaded JSON data into a Pandas DataFrame.
- Inspected data structure and handled missing values.
2. Text Preprocessing
- Converted text to lowercase
- Removed punctuation
- Removed special characters
- Removed words containing numbers
- Lemmatization
- POS tagging and noun extraction
- Created a clean complaint corpus
3. Exploratory Data Analysis (EDA)
- Complaint length distribution
- Word frequency analysis
- Word cloud visualization
- Unigram, Bigram, and Trigram analysis
4. Feature Extraction
- TF-IDF Vectorization
- Text-to-feature transformation for topic modeling and classification
5. Topic Modeling

Applied Non-Negative Matrix Factorization (NMF) to identify latent complaint topics.

Discovered topics were mapped to the following categories:

- Credit Card / Prepaid Card
- Bank Account Services
- Theft / Dispute Reporting
- Mortgages / Loans
- Others
6. Supervised Learning

Created a labeled dataset using NMF-generated topics and trained multiple classifiers:

- Logistic Regression
- Multinomial Naive Bayes
- Decision Tree Classifier
- Random Forest Classifier
7. Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Classification Report
- Confusion Matrix
8. Prediction

The final model can classify unseen customer complaints into the appropriate business category.

- Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- spaCy
- Scikit-learn
- WordCloud

Results
- Successfully identified complaint topics using NMF.
- Generated labeled data from unsupervised topic modeling.
- Trained and compared multiple classification models.
- Automated routing of customer complaints into business-specific categories.

Author

Kavya Kumar Bhalia

B.Tech CSE (AI & ML)
Rayat Bahra University