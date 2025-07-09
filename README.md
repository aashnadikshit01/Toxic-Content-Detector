# Toxic-Content-Detector
The aim of this notebook is to implement a robust pipeline for detecting harmful/toxic content from social media platforms using traditional NLP methods. I will use TF-IDF vectorization and train multiple scikit-learn models to compare their performance on binary classification tasks.

This the the data set that was used: https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge

Here's what was accomplished:

1. Built a complete pipeline from data preprocessing to model deployment
2. Compared multiple classical ML models
3. Created a reusable prediction function
4. Saved our best model for future use

Potential improvements:
1. Adding more features like sentiment scores
2. Implementing cross-validation for more robust evaluation
3. Creating a simple web interface using Flask/Streamlit

To use this model in production:
1. Load the saved model and vectorizer:
```
model = joblib.load('best_model.joblib')
vectorizer = joblib.load('tfidf_vectorizer.joblib')
```

2. Use the predict_toxicity function:
```
result = predict_toxicity("your text here", model, vectorizer)
```
