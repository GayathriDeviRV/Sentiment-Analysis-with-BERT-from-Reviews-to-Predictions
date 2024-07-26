# Sentiment-Analysis-with-BERT-from-Reviews-to-Predictions

This project involves sentiment analysis on women's clothing e-commerce reviews using BERT (Bidirectional Encoder Representations from Transformers). The goal is to classify reviews into three sentiment categories: Positive, Neutral, and Negative.

## Project Overview

The dataset contains 23,486 customer reviews of women's clothing items, with features such as the review text, rating, and more. This project preprocesses the data, balances the class distribution, and fine-tunes a pre-trained BERT model to classify the sentiment of the reviews.

## Key Steps

1. **Data Preprocessing:**
   - Loaded the dataset and handled null values.
   - Defined sentiment labels based on the rating:
     - Positive (4-5)
     - Neutral (3)
     - Negative (1-2)

2. **Exploratory Data Analysis (EDA):**
   - Visualized the distribution of sentiments and ratings.
   - Analyzed the length of reviews.

3. **Data Balancing:**
   - Used RandomOverSampler to balance the sentiment distribution.

4. **Model Training (Fine-Tuning BERT):**
   - Tokenized the reviews using BERT tokenizer.
   - Split the data into training and testing sets.
   - Fine-tuned a pre-trained BERT model for sequence classification on the dataset.

5. **Evaluation:**
   - Evaluated the model using accuracy, precision, recall, and F1-score.
   - Displayed the confusion matrix.

6. **Inference:**
   - Predicted sentiments of new reviews using the trained model.

## Results

The model achieved an accuracy of 94.23% on the test set.

## Acknowledgment

- The dataset was sourced from Kaggle: [Women's Clothing E-Commerce Reviews](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews)
