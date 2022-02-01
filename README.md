![](https://github.com/PrachiPatel15/Fake-News-Detection/blob/main/wordcloud.png)

# Fake-News-Detection: Project Overview
- In this data science project idea, we will use Python to build a model that can accurately detect whether a piece of news is real or fake.
- We've build TfidfVectorizer and used different classifier to classify between "Real" and "Fake" news.
- In this project, for optimization we've used __3__ different machine learning model.
- Using different classifiers, we've reached to optimal solution.

# Code and Resources Used
- ***Python Version:*** 3.8
- ***Packages:*** pandas, sklearn, matplotlib, pipeline, seaborn
- ***Dataset:*** https://www.kaggle.com/umarfarooq45/fake-news-and-true-news

# Data
- In this project, we have 2 different datasets named __"Fake.csv"__ and __"True.csv"__ and both datasets have below attributes:
  - title
  - text
  - subject
  - date
 - We merged both datasets and added 'Target' column to classify which is true news or fake.

# Data Cleaning
- Raw dataset needed to be cleaned up little.
- Firstly, we dropped 'title' and 'date' columns so new dataset has below attributes.
  - text
  - subject
  - Target
- Then we shuffled the data for exploration.
- And lastly We removed punctuations and stopwords from the 'text' column.

# Basic Data Exploration
- Created wordcloud for fake and true news.
- We checked the most frequent words in both the news and plotted the graph for both.

# Model Building
- I tried three different models and  evaluated them using f1-score and confusion matrix.
  - LogisticRegression -basline
  - Decision Tree Classifier
  - Random Forest Classifier

# Model Performance
- LogisticRegression : f1-score = 0.98
- Decision Tree Classifier : f1-score = 0.99
- Random Forest Classifier : f1-score = 0.99

- ![confusion matrix of Random Forest Classifier:](https://github.com/PrachiPatel15/Fake-News-Detection/blob/main/confusion(RF).png)

