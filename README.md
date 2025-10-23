# Sentiment Analysis — Review Classification App

## Project Vision
This project aims to build a **mobile application** that performs **sentiment analysis** on user reviews using **Natural Language Processing (NLP)** and **Machine Learning (ML)**.  
The system will classify text as **Positive**, **Negative**, or **Neutral**, helping users or companies understand opinions about a product or service more easily.  
It will also demonstrate how deep learning methods can be applied in real-world natural language tasks.

---

## Title and Short Description
**Title:** Sentiment Analysis  

**Short Description:**  
This project creates a mobile app that can identify the emotional tone of written reviews.  
It combines a Python-based backend model and a Flutter/Android frontend.  
The app processes text input, predicts the sentiment, and shows the result with a simple and friendly interface.  

---

## Platform and Tools
- **Languages:** Python (for model), Java / Flutter (for mobile app)  
- **Backend Framework:** Flask / FastAPI  
- **Frontend Framework:** Flutter / Android Studio  
- **Tools:** GitHub, VS Code, Jupyter Notebook, Google Colab  

---

## Dataset
The project will use open-source datasets such as:  
- [Amazon Product Review Dataset (Kaggle)](https://www.kaggle.com/datasets/bittlingmayer/amazonreviews)  
- [IMDB Movie Reviews Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)  

Each dataset includes a review and its label (positive, negative, or neutral).  
Before training, data will be cleaned and balanced to improve model quality.

---

## Methods
1. **Text Preprocessing** – tokenization, stop-word removal, lemmatization.  
2. **Feature Extraction** – TF-IDF, Word2Vec, or BERT embeddings.  
3. **Model Training** – Logistic Regression, SVM, LSTM, or fine-tuned BERT.  
4. **Evaluation** – Accuracy, Precision, Recall, and F1-score.  
5. **Deployment** – Model will be integrated into the app through an API using Flask or FastAPI.

---

## App Features
| Feature | Description |
|----------|-------------|
| **Text Input** | Users can type or paste a review for analysis. |
| **Sentiment Prediction** | Shows whether the text is Positive, Negative, or Neutral. |
| **Visual Display** | Simple pie or bar chart of the sentiment result. |
| **History** | Option to save and view past results. |
| **Settings** | Allows theme and language selection. |

---

## Security and Ethics
- Uses open-source, anonymised datasets only.  
- No user data will be stored or shared.  
- Follows the **UEA Research Ethics Policy** and **GDPR (2018)**.  
- Ethical approval will be obtained before any data collection or processing.  

---

## Project Timeline
| Phase | Description | Duration |
|-------|--------------|-----------|
| 1 | Literature Review and Dataset Collection | Month 1–2 |
| 2 | Model Training and Testing | Month 3–5 |
| 3 | App Development and Integration | Month 6–8 |
| 4 | Evaluation and Optimisation | Month 9–10 |
| 5 | Final Report and Presentation | Month 11–12 |

---

## Supervisor
**Dr Farhana Liza**  
School of Computing Sciences, University of East Anglia  

---

## Expected Outcome
By the end of this project, there will be a working mobile app that can predict the sentiment of a given text.  
It will show how NLP and machine learning can be combined to create intelligent, user-focused tools.

---

## Future Work
- Add multilingual support for analysing non-English text.  
- Improve model accuracy using newer transformer-based models.  
- Explore on-device deployment for offline use.

---
