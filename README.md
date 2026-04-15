# News-Category-Classification-

This project focuses on building a News Category Classification system that automatically classifies news articles into one of four categories:

🌍 World
🏅 Sports
💼 Business
🔬 Sci/Tech

The goal is to apply Natural Language Processing (NLP) techniques and compare different machine learning models to achieve high classification performance.

📊 Dataset

The dataset consists of news articles with the following fields:

Title
Description
Class Index (Label)

The text data is preprocessed by:

Expanding contractions
Lowercasing text
Removing URLs, mentions, and special characters
Lemmatization
Stopword removal (with preservation of important negations)

Finally, the title and description are combined to form a single input feature for training.

⚙️ Feature Extraction
TF-IDF Vectorization is used to convert text into numerical features:
TfidfVectorizer(stop_words="english")
🤖 Machine Learning Models

Two classification models were trained and evaluated:

🌲 Random Forest Classifier
Ensemble-based model
Handles non-linear patterns well

Performance:

Accuracy: 90%
Weighted F1-score: 0.90
Class	Precision	Recall	F1-score
World	0.92	0.89	0.90
Sports	0.93	0.98	0.95
Business	0.86	0.85	0.86
Sci/Tech	0.87	0.86	0.87
📈 Logistic Regression
Strong linear classifier for high-dimensional text data
Performs very well with TF-IDF features

Performance:

Accuracy: 91%
Weighted F1-score: 0.91
Class	Precision	Recall	F1-score
World	0.93	0.90	0.91
Sports	0.95	0.98	0.97
Business	0.88	0.88	0.88
Sci/Tech	0.89	0.90	0.89
🏆 Results Summary
Model	Accuracy	Best Performance
Random Forest	90%	Good baseline
Logistic Regression	91%	Best overall

👉 Logistic Regression slightly outperforms Random Forest on this dataset.

🚀 Key Insights
TF-IDF + Linear models work extremely well for text classification
Logistic Regression is highly effective for sparse high-dimensional data
Class distribution is balanced, making evaluation reliable
Simple preprocessing + classical ML models can achieve strong results without deep learning
🧠 Tools & Libraries
Python
Scikit-learn
NLTK
Pandas
NumPy
📌 Conclusion

This project demonstrates that traditional machine learning models combined with proper NLP preprocessing can achieve strong performance in text classification tasks, making them a reliable and efficient solution for real-world news categorization systems.
