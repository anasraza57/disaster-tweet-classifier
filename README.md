# Disaster Tweet Classifier 🧠📉

This project is part of the CSC-40070 coursework at Keele University. It focuses on classifying tweets during natural disasters using machine learning and deep learning techniques. The aim is to support emergency response efforts by filtering relevant information from large volumes of social media data.

## 📁 Dataset

- Source: [Kaggle - Real or Not? NLP with Disaster Tweets](https://www.kaggle.com/competitions/nlp-getting-started)
- Size: 7,613 labelled tweets
- Labels:  
  - `1` = Disaster-related  
  - `0` = Not disaster-related

## 🧹 Preprocessing

- Lowercasing
- Removing URLs, mentions, hashtags, punctuation
- Stopword removal (using NLTK)
- Lemmatization
- Duplicate and empty row removal

## 🧠 Models Used

### 1. Logistic Regression  
- Baseline model using TF-IDF vectors

### 2. Support Vector Machine (SVM)  
- Better suited for high-dimensional text data

### 3. Long Short-Term Memory (LSTM)  
- Bidirectional model trained on padded sequences  
- Applied class weighting and early stopping to handle imbalance and overfitting  
- Achieved ~80% accuracy

## 📊 Visualisations

- Class distribution bar chart  
- Word clouds for disaster and non-disaster tweets  
- Tweet length histogram  
- Confusion matrix for LSTM predictions

## ⚙️ Libraries Used

- `pandas`, `numpy`, `scikit-learn`  
- `nltk`, `seaborn`, `matplotlib`, `wordcloud`  
- `tensorflow.keras`

## 📂 Structure

- `disaster_tweet_model.ipynb` – Full notebook with preprocessing, modelling, and evaluation  
- `cleaned_disaster_tweets.csv` – Preprocessed dataset  
- `report.pdf` – Final report with findings, results, and visualisations

## ✅ Results

- **LSTM Model Accuracy**: 80%  
- Strong balance between precision and recall  
- Outperformed traditional models on contextual understanding of tweets

## 📄 License

This project is academic coursework. Dataset is publicly available via Kaggle.

