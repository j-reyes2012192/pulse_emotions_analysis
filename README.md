This project explores sentiment analysis by leveraging various data processing and visualization techniques. The aim is to analyze movie reviews and classify them as positive or negative with high accuracy.

Project Overview
Objective: Train a sentiment analysis model to detect negative reviews with an F1 score of at least 0.85.
Dataset: IMDB movie reviews from 1894 to 2010 with polarity legends.

Key Components
Data Initialization and Exploration:

Dataset includes review, pos (target column), and ds_part (data split indicator).
Missing values in average_rating and votes.
Object type columns for end_year and runtime_minutes.
Exploratory Data Analysis (EDA):

Trends in reviews and movies over time.
Review distribution per movie.
Positive and negative review distributions across dataset parts.
Evaluation Procedure:

Custom evaluation routine for all models.
Text normalization applied to ensure compatibility across models.
Model Development:

Model 0 (Baseline): Dummy classifier for reference.
Model 1: Logistic Regression with NLTK tokenization and TF-IDF.
Model 2: Logistic Regression with spaCy tokenization and TF-IDF.
Model 3: LGBMClassifier with GridSearchCV using spaCy and TF-IDF.
Testing New Reviews:

Model performance validated on unseen reviews.
Results
Models achieved F1 scores above 0.85.
Best Performer: Model 1 (Logistic Regression with NLTK and TF-IDF).
Conclusions
Logistic Regression models performed well across metrics.
Further refinement could enhance predictions for ambiguous reviews.
