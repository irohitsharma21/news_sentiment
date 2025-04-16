📰 News Sentiment Analysis

🎯 Objective
Classify news headlines into Positive, Negative, or Neutral sentiments using ML and NLP techniques.

📊 Dataset
Source: Kaggle
Text: News headlines
Labels: Positive, Negative, Neutral
Slight class imbalance (more Neutral samples)

🧹 Preprocessing
Removed nulls, lowercased text
Cleaned punctuation & digits (Regex)
Tokenized & lemmatized (nltk, spaCy)
Removed stopwords
Label-encoded sentiments

🧠 Models Used
Classical: Logistic Regression, Naive Bayes, SVM (best among these)
Deep Learning: LSTM with Keras
Transformer: Fine-tuned BERT (best overall) using HuggingFace

📈 Evaluation
Metrics: Accuracy, Precision, Recall, F1 Score
BERT had highest F1 score, SVM was a strong classical alternative
Visuals: Loss vs Accuracy plots (LSTM, BERT), Confusion Matrix

⚠️ Challenges
Class imbalance → used class weights
LSTM overfitting → handled with dropout & early stopping
BERT training needs GPU → used Colab

✅ Conclusion
BERT delivered the best results. SVM worked well for faster, low-resource scenarios. The pipeline is solid for scaling or real-time use.
