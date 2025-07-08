 #👨‍🚒Natural-Language-Preprocessing-and-Modelling-with-Disaster-tweets
# 👨‍🚒Natural Language Preprocessing and Modelling with Disaster Tweets

☘️**Goal:**  We use real-time tweet classification to identify disaster-related content, which serves as a foundational tool for building an early warning system based on tweet social media signals.

☘️**Dataset:** The dataset provides about 10,000 labeled tweets, and the task is to classify each tweet into two categories: disaster (1) or non-disaster (0).

☘️**Methods:** 

(1) Natural Language preprocessing the text

(2) Exploratory Data Analysis

(3) Modelling 

(4) Evaluation of Models

(5) Improvement Analysis

☘️**Techniqual Used:**

(1) Text preprocessing and Visualization( nltk, re , seaborn, matpoltlib)

(2) EDA (wordcloud, collections)

(3) Data splitting and Randomization(sklearn)

(4) Text Vectorization (sklearn)

(5) Modelling (sklearn, xgboost)
  Logistic Regression, 
  Random Forest Model, 
  XGBoost Model 
  SVC Model
  
(6) Evaluation(sklearn)

(7) Improvemnet of the Modelling(sklearn.pipeline, scipy)

☘️**Key Finding:**

| **Tuning Strategy**                                    | **Recall (Class 1)** | **Accuracy** | **Precision (Class 1)** | **F1 Score (Class 1)** | **Remarks**                                                                |
| ------------------------------------------------------ | -------------------- | ------------ | ----------------------- | ---------------------- | -------------------------------------------------------------------------- |
| **Baseline** *(Original Logistic Regression)*          | 0.69                 | 82.7%        | 0.88                    | 0.77                   | Highest accuracy, but lower recall for disasters                           |
| **Class Weight Only**                                  | 0.74 ↑               | 78.99% ↓     | —                       | 0.75                   | Improves disaster sensitivity; slight drop in accuracy                     |
| **Threshold = 0.4 Only**                               | 0.77 ↑               | 77.3% ↓      | 0.72 ↓                  | 0.75                   | Good balance, more disaster tweets caught                                  |
| **Add Features (alert terms, length, negative words)** | 0.76 ↑               | 80.4% ↓      | 0.78 ↓                  | 0.77                   | Improves recall; slight drop in accuracy and precision                     |
| **Class Weight + Threshold = 0.4**                     | **0.82** ↑           | **74.7%** ↓  | 0.67 ↓                  | 0.74                   | Highest recall; largest drop in accuracy; useful for early warning systems |




