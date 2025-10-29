# 🎬 Sentiment Analysis on IMDB Movie Reviews  
**CS412 – Machine Learning (Spring 2025)**  
📚 **Sabancı University**  

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.5-green.svg)
![License](https://img.shields.io/badge/License-Academic-lightgrey.svg)

---

## 🧠 Overview  
This project focuses on **binary sentiment classification** using the **IMDB movie reviews dataset**.  
The task: determine whether a given review expresses a **positive** or **negative** sentiment.  

We compare three different paradigms of text classification:  

| Model | Approach | Description |
|:------|:----------|:-------------|
| 🧩 Logistic Regression (TF-IDF) | Traditional ML | Simple, interpretable baseline using statistical text features |
| 🔁 LSTM (Long Short-Term Memory) | Deep Learning | Captures sequential word dependencies and contextual relationships |
| ⚡ CNN (Convolutional Neural Network) | Deep Learning | Learns local sentiment cues and n-gram patterns efficiently |

Our goal was to explore how **classical vs. deep learning** approaches differ in accuracy, interpretability, and computational trade-offs.

---

## 🧩 Problem Definition  
- **Type:** Binary Classification  
- **Input:** Textual movie reviews  
- **Output:** Sentiment label → `positive` (1) or `negative` (0)  
- **Dataset Size:** 50,000 reviews (balanced)  
- **Challenge:** Handle diverse review lengths, idiomatic language, and long-range dependencies  

---

## 📊 Dataset  
- **Source:** [IMDB Movie Reviews](https://ai.stanford.edu/~amaas/data/sentiment/)  
- **Samples:** 25,000 positive + 25,000 negative reviews  
- **Average Length:** ~230 words/review  
- **Format:**
  ```text
  review,sentiment
  "This movie was absolutely wonderful...",positive
  "Terrible pacing and awful acting.",negative
