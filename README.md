📊 Sentiment Analysis using Machine Learning

This project focuses on building a complete Sentiment Analysis pipeline that classifies customer reviews into Positive, Neutral, or Negative sentiments using Natural Language Processing and Machine Learning.

The project demonstrates the end-to-end workflow of a real NLP project — from raw data preprocessing to model evaluation and performance analysis.

🎯 Project Objective

Customer reviews contain valuable insights for businesses. This project aims to:

Automatically analyze customer reviews

Identify customer sentiment from text

Compare multiple ML models

Build a highly accurate sentiment classifier

The final model helps businesses understand customer satisfaction and make data-driven decisions.

📁 Project Files
File	Description
Sentiment Analysis.ipynb	Full step-by-step workflow and visualization
Sentiment Analysis.py	Script version of the notebook
Dataset (CSV)	Amazon Musical Instrument Reviews
⚙️ Environment & Tools

The project is built using Python and Jupyter Notebook.

Libraries Used
Data Handling

Pandas

NumPy

Visualization

Matplotlib

WordCloud

Natural Language Processing

NLTK

TextBlob

Machine Learning

Scikit-learn

Imbalanced-learn (SMOTE)

📦 Dataset Description

The dataset contains customer reviews of musical instruments.

Each record includes:

Review text

Review summary

Product rating (1–5 stars)

Additional metadata

Dataset Size:

10,261 reviews

9 original columns

🧹 Data Preprocessing

Real-world text data is messy. A full cleaning pipeline was implemented.

1️⃣ Handling Missing Values

Missing review text replaced with empty strings.

2️⃣ Feature Creation

Review text and summary were combined into a single column called reviews.

3️⃣ Sentiment Label Creation

Ratings were converted into sentiment labels:

Rating	Sentiment
> 3	Positive
= 3	Neutral
< 3	Negative

This converts the problem into a multi-class classification task.

🔤 Text Preprocessing Pipeline

Text preprocessing is the most important step in NLP.

Cleaning Steps

Convert text to lowercase

Remove punctuation

Remove numbers

Remove links and newlines

Text Processing

Tokenization

Stopword removal (keeping “not” for negation)

Lemmatization

This improves model understanding and reduces noise.

📊 Exploratory Data Analysis (EDA)

Several analyses were performed to understand the data.

Key Observations

Majority reviews are positive

Reviews are typically short

Dataset is imbalanced

Additional Features Generated

Text polarity (TextBlob)

Review length

Word counts

These help understand text distribution and sentiment behavior.

🔎 N-Gram Analysis

To understand commonly used words:

Unigram analysis (single words)

Bigram analysis (two-word phrases)

Trigram analysis (three-word phrases)

This helps identify common positive and negative phrases.

☁️ Word Cloud Visualization

Word clouds were generated for:

Positive reviews

Neutral reviews

Negative reviews

This visually highlights frequently used words.

🛠 Feature Engineering
1️⃣ Removing Irrelevant Columns

Columns not useful for prediction were removed.

2️⃣ Label Encoding

Sentiments converted to numbers:

Positive → 2

Neutral → 1

Negative → 0

3️⃣ TF-IDF Vectorization

Text converted into numeric features using:

5000 bigram features

This transforms text into machine-readable format.

⚖️ Handling Imbalanced Dataset

The dataset had far more positive reviews than negative ones.

To fix this:

SMOTE (Synthetic Minority Oversampling) was used.

This balanced the dataset and improved model fairness.

✂️ Train-Test Split

Dataset split into:

75% Training

25% Testing

🤖 Machine Learning Models Tested

Multiple models were compared using 10-Fold Cross Validation:

Decision Tree

Logistic Regression

Support Vector Machine

Random Forest

Naive Bayes

K-Nearest Neighbors

Best Model

👉 Logistic Regression performed best

⚙️ Hyperparameter Tuning

GridSearchCV was used to find the best parameters for Logistic Regression.

This step improved model performance significantly.

📈 Model Performance
Final Results
Metric	Score
Accuracy	~95%
F1 Score	~95%
Confusion Matrix Insight

Model predicts positive and neutral reviews very well.

Slight difficulty detecting negative reviews (due to original imbalance).

🏁 Conclusion
Dataset Insights

Most reviews are positive.

Guitar-related products dominate discussions.

Text preprocessing strongly improves model performance.

Model Insights

Logistic Regression is highly effective for text classification.

SMOTE improved detection of minority classes.

Final model achieves excellent accuracy and reliability.

🚀 Skills Demonstrated

Natural Language Processing (NLP)

Data Cleaning & Preprocessing

Exploratory Data Analysis

Feature Engineering

Imbalanced Data Handling

Machine Learning Model Comparison

Hyperparameter Tuning

Model Evaluation
