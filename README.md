# Sentiment Analysis and Named Entity Recognition in Restaurant Reviews

Final project for the **Text Mining** course at ISCTE, focusing on **automated sentiment classification** and **named entity recognition (NER)** in restaurant reviews extracted from TripAdvisor, specifically for establishments in Lisbon.

---

## Project Objectives

- Automatically classify the **sentiment** of textual reviews on a 1–5 rating scale.
- Identify **employee names** in the text and detect when they are being **complimented**.
- Analyze **inconsistencies** between the written content and the numerical rating given by the user.

---

## Technologies and Libraries

- Python 3.x  
- [Selenium](https://www.selenium.dev/) – Web scraping  
- [spaCy](https://spacy.io/) – NLP and Named Entity Recognition  
- [scikit-learn](https://scikit-learn.org/) – ML models  
- [Keras / TensorFlow](https://keras.io/) – Neural network  
- [Transformers (HuggingFace)](https://huggingface.co/) – BERT  
- [NLTK](https://www.nltk.org/) – Preprocessing utilities  
- Google Colab – For GPU-based model training  
---

## Key Results

### Binary classification (Positive vs. Negative):

Logistic Regression: F1 ≈ 0.92, Accuracy ≈ 0.92

Naive Bayes: F1 ≈ 0.80

### Multiclass sentiment classification (1–5 rating):

Neural Network (custom embeddings): Accuracy ≈ 62%

BERT-based model: Accuracy ≈ 54% - Implementation can be improved

Random Forest with language flag: Accuracy ≈ 54%

### NER + Compliment detection:

Used spaCy models (pt_core_news_lg, en_core_web_lg)

Detected and ranked employees based on positive context

---

## Future Work

Expand dataset to more restaurants and cities

Refine BERT aplication

Build an interactive dashboard for managers

Create a REST API for online inference or integration with platforms like TripAdvisor

---

## How to Run

1. **Install dependencies**:

```bash
pip install -r requirements.txt