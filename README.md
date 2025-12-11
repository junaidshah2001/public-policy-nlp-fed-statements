# NLP Analysis of Federal Reserve (FOMC) Statements

This project conducts a full Natural Language Processing (NLP) workflow on Federal Reserve (FOMC) policy statements to uncover themes, sentiment patterns, uncertainty levels, and their relationship with financial market volatility. Using topic modelling, dictionary-based sentiment metrics, and regression analysis, the project demonstrates how central bank communication can be quantified and interpreted using data science methods.

---

## 📌 Project Objectives

This project focuses on four core analytical goals:

1. **Clean and preprocess FOMC policy statements** to create a structured corpus.  
2. **Extract features** using Bag-of-Words and TF–IDF representations.  
3. **Identify themes/topics** using NMF and LDA topic modelling.  
4. **Measure sentiment, negativity, and uncertainty** in central bank communication.  
5. **Study how text-based indicators relate to financial market volatility** through regression.

---

## 🧹 Part 1 — Text Preprocessing

The preprocessing pipeline includes:

- Lowercasing text  
- Removing punctuation and extra spacing  
- Removing digits  
- Removing stopwords  
- Lemmatization  
- Filtering out short or meaningless tokens  

This ensures a clean and consistent corpus from which meaningful patterns can be extracted.  
An early inspection of the statements reveals common policy-related vocabulary such as **“inflation,” “employment,” “economic conditions,” “rates,”** and **“growth.”**

---

## 🧾 Part 2 — Feature Extraction

Two feature extraction methods are used:

### **1. Bag-of-Words (BoW)**  
Captures raw term frequencies across all statements.

### **2. TF–IDF**  
Weights terms by importance across the document set, reducing the influence of overly common words.

Both representations are used for topic modelling.

---

## 🧩 Part 3 — Topic Modelling (NMF & LDA)

Two topic modelling approaches are implemented:

### **🔷 Non-negative Matrix Factorization (NMF)**  
Key characteristics:
- Learns *parts-based* representations  
- Produces interpretable weighted topic-word relationships  
- W matrix → topic weights per document  
- H matrix → word weights per topic  

### **🔶 Latent Dirichlet Allocation (LDA)**  
A probabilistic generative model that estimates:
- **θ (theta)** → topic distribution for each document  
- **β (beta)** → word distribution for each topic  

---

## 🎨 Topic Visualization

Both NMF and LDA topic distributions were visualized to understand the most significant themes in FOMC communication.

While the notebook does not contain a textual printed list of topics, visual inspection of topic-word distributions shows recurring themes such as:

- Economic growth and output  
- Employment and labor markets  
- Inflation pressures  
- Monetary policy stance  
- Financial stability and credit conditions  

These themes align with typical central bank communication structure.

---

## 📊 Part 6 — Sentiment, Negativity & Uncertainty

Sentiment analysis is performed using a dictionary-based approach tailored for financial and policy text.

Metrics extracted include:

- **Positive sentiment**  
- **Negative sentiment**  
- **Uncertainty words**  
- **Constraining/modality language**

These metrics capture how the tone of policy communication changes over time, highlighting shifts during periods of:

- Economic uncertainty  
- Financial market stress  
- Shifts in policy direction  

---

## 📉 Part 10 — Regression Analysis

A regression model explores the relationship between:

- **Uncertainty in FOMC statements**, and  
- **Financial market volatility (VIX)**

The key finding from the model:

### ✅ **Finding (From Notebook Output)**  
> *There is evidence that higher uncertainty in FOMC statements is associated with increased stock market volatility.*

### ⚠️ Issue  
The model is extremely simple and underspecified.  
Volatility is affected by many external factors, so further variables would improve the model.

However, the analysis successfully demonstrates how textual uncertainty can be linked to market reactions.

---

##Download NLTK resources:

import nltk
**nltk.download('stopwords')
**nltk.download('wordnet')

🎯 Key Skills Demonstrated

End-to-end NLP pipeline

Advanced text preprocessing

Topic modelling (NMF & LDA)

Topic coherence evaluation

Sentiment & uncertainty analysis

Data visualization

Regression using text-based features

Applied financial/policy analytics

✍️ Author

Muhammad Junaid Shah Bukhari
Public Administration & Governance • Data Science & NLP

linkedin: https://www.linkedin.com/in/junaidshah2001/
Kaggle: https://www.kaggle.com/junaid2101
