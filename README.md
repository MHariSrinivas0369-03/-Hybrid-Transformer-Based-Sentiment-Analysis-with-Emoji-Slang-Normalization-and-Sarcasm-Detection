# A Hybrid Transformer-Based Sentiment Analysis Model with Emoji-Slang Normalization and Sarcasm Detection

## 📌 Overview

This project presents a hybrid sentiment analysis framework designed to improve sentiment classification on social media text. The proposed system combines the strengths of transformer-based deep learning, traditional machine learning, sequential neural networks, and sarcasm detection to accurately classify sentiments expressed in noisy and informal social media content.

The framework integrates DistilBERT for contextual understanding, TF-IDF with Logistic Regression for lexical feature extraction, BiLSTM for sequential learning, and a RoBERTa-based sarcasm detector to identify ironic expressions. By combining these models through a weighted ensemble mechanism, the system achieves robust and reliable sentiment predictions.

---

## 🎯 Objectives

- Improve sentiment classification accuracy on social media data.
- Handle emojis, slang expressions, and informal language.
- Detect sarcasm and adjust sentiment polarity accordingly.
- Combine contextual, lexical, and sequential learning approaches.
- Build a scalable and interpretable sentiment analysis framework.

---

## 🏗️ System Architecture

The proposed framework consists of four major components:

### 1. DistilBERT (Transformer Expert)
- Captures contextual meaning and semantic relationships.
- Fine-tuned on the Sentiment140 dataset.
- Provides deep contextual sentiment understanding.

### 2. TF-IDF + Logistic Regression
- Extracts lexical features from text.
- Provides interpretable sentiment predictions.
- Acts as a strong statistical baseline.

### 3. BiLSTM (Sequential Expert)
- Learns word-order dependencies.
- Captures sequential contextual information.
- Enhances understanding of sentence structure.

### 4. RoBERTa-Based Sarcasm Detector
- Detects sarcasm and irony in tweets.
- Adjusts sentiment predictions when sarcastic content is identified.

---

## 🔄 Workflow

```text
Input Tweet
      │
      ▼
Emoji & Slang Normalization
      │
 ┌────┼────┐
 │    │    │
 ▼    ▼    ▼
DistilBERT  TF-IDF+LR  BiLSTM
 │      │      │
 └──────┼──────┘
        ▼
 Weighted Ensemble
        │
        ▼
 Sarcasm Detection
        │
        ▼
Final Sentiment Prediction
```

---

## 📊 Dataset

**Dataset Used:** Sentiment140

### Dataset Features
- 1.6 Million labeled tweets
- Positive and Negative sentiment labels
- Real-world social media content
- Rich in emojis, hashtags, abbreviations, and slang

### Training Configuration
| Model | Training Samples |
|---------|----------------|
| DistilBERT | 800,000 Tweets |
| Logistic Regression | 50,000 Tweets |
| BiLSTM | 50,000 Tweets |

---

## 🛠️ Technologies Used

| Category | Technology |
|-----------|------------|
| Programming Language | Python |
| NLP Models | DistilBERT, RoBERTa |
| Deep Learning | PyTorch |
| Machine Learning | Scikit-Learn |
| Sequential Modeling | BiLSTM |
| Feature Engineering | TF-IDF |
| Dataset | Sentiment140 |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib |

---

## ✨ Key Features

- Transformer-based contextual sentiment understanding
- Emoji and slang normalization
- Sarcasm-aware sentiment prediction
- Hybrid ensemble architecture
- Confidence score generation
- Real-time sentiment inference
- Explainable multi-model predictions

---

## 📈 Performance Results

| Model | Accuracy |
|---------|----------|
| Logistic Regression (TF-IDF) | 78.19% |
| BiLSTM | 74.02% |
| DistilBERT | 86.56% |
| Hybrid Ensemble | **86.58%** |

The Hybrid Ensemble model achieved the highest accuracy by combining lexical, contextual, and sequential representations while reducing classification errors.

---

## 📋 Sample Applications

- Social Media Monitoring
- Brand Reputation Analysis
- Customer Feedback Analysis
- Market Research
- Product Review Classification
- Public Opinion Tracking
- Real-Time Sentiment Monitoring

---

## 🚀 Future Enhancements

- Multilingual sentiment analysis support
- Fine-grained emotion classification
- Real-time social media streaming integration
- Explainable AI dashboards
- Multimodal sentiment analysis using text and images

---


## 👨‍💻 Authors

**M. Hari Srinivas**  
Department of Big Data Analytics  
Vellore Institute of Technology (VIT)

**B. Hemanth Kumar**  
Department of Big Data Analytics  
Vellore Institute of Technology (VIT)

**S. Govardhan**  
Department of Big Data Analytics  
Vellore Institute of Technology (VIT)

**Dr. R. Manjula**  
School of Computer Science and Engineering  
Vellore Institute of Technology (VIT)

---

## 📄 Publication

**A Hybrid Transformer-Based Sentiment Analysis Model with Emoji-Slang Normalization and Sarcasm Detection**

Conference Research Project developed at Vellore Institute of Technology (VIT).

---

## ⭐ Project Highlights

- Hybrid AI Architecture
- Transformer + BiLSTM + Logistic Regression Ensemble
- Sarcasm-Aware Sentiment Analysis
- Emoji and Slang Normalization
- Context-Aware Social Media Analytics
- 86.58% Classification Accuracy
