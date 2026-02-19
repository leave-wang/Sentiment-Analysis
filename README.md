1. Project Vision
This project aims to design and implement a sentiment analysis system that not only classifies user reviews as Positive, Negative, or Neutral, but also improves reliability by reducing misattributed negative sentiment through a novel smoothing approach inspired by NSSM (Negative Sentiment Smoothing Mechanism).
The system integrates:
Natural Language Processing (NLP)
Machine Learning (ML)
A rule-based smoothing module
A mobile application interface
The goal is to explore whether sentiment reliability can be improved by adjusting negative signals that are unrelated to the main target entity.
2. Research Question
Does applying a Negative Sentiment Smoothing mechanism improve sentiment classification performance and reliability compared to standard baseline models?
Sub-questions:
How does smoothing affect classification metrics?
Does smoothing reduce false negatives?
How sensitive is performance to the smoothing parameter β?
This transforms the project from a simple app into a research-based investigation.
3. Title and Description
Title:
Entity-Aware Sentiment Analysis with Negative Sentiment Smoothing
Short Description:
This project builds a mobile sentiment analysis application powered by a Python backend. The system uses machine learning models (TF-IDF + Logistic Regression / SVM) and integrates an NSSM-based smoothing module to improve classification reliability. The backend is deployed via FastAPI and connected to a Flutter-based frontend.
4. Platform and Tools
Backend:
Python
Scikit-learn
spaCy
VaderSentiment
FastAPI
Frontend:
Flutter / Android Studio
Development Tools:
GitHub
VS Code
Jupyter Notebook
Google Colab
5. Dataset
Primary Dataset:
IMDB Movie Review Dataset (binary classification)
Optional Extension:
Amazon Product Reviews Dataset (multi-class)
Each dataset contains:
Review text
Sentiment label
Data processing includes:
Cleaning and normalization
Lowercasing
Stopword removal (for ML baseline)
Train/Test split
Optional class balancing
6. Methodology
6.1 Baseline Models
The following baseline models will be implemented:
Vader Sentiment (rule-based baseline)
TF-IDF + Logistic Regression
TF-IDF + SVM (optional extension)
Evaluation Metrics:
Accuracy
Precision
Recall
F1-score
Confusion Matrix
6.2 Negative Sentiment Smoothing (NSSM)
A smoothing mechanism is applied after baseline sentiment scoring.
Steps:
Split text into sentences using spaCy.
Detect negative sentences using Vader.
Identify negative sentences unrelated to the target entity.
Adjust overall sentiment score using:
S
a
d
j
u
s
t
e
d
=
S
0
+
β
⋅
n
S 
adjusted
​	
 =S 
0
​	
 +β⋅n
Where:
S
0
S 
0
​	
  = base compound sentiment score
n
n = number of unrelated negative sentences
β
β = smoothing parameter
The parameter β will be experimentally tuned.
6.3 Experimental Design
Experiments include:
Baseline vs NSSM comparison
Beta parameter sweep (0.05, 0.1, 0.2, 0.3)
Error analysis of misclassified reviews
Ablation study (with and without entity filtering)
This ensures the project demonstrates research depth rather than simple implementation.
7. System Architecture
User Input (Mobile App)
→ API Request (FastAPI)
→ ML Model Prediction
→ NSSM Adjustment
→ Response JSON
→ Frontend Display
The backend exposes endpoints:
/predict
/history
/model-switch
8. App Features
Feature	Description
Text Input	Users can type or paste a review
Sentiment Prediction	Displays Positive / Negative / Neutral
Probability Score	Shows model confidence
Visualization	Bar chart for sentiment score
History	Save and view past predictions
Model Switch	Choose baseline or NSSM
Settings	Theme and language selection
9. Security and Ethics
Uses anonymised open-source datasets only
No personal user data stored permanently
GDPR compliant (2018)
Ethical approval obtained if required
Model bias discussion included in report
10. Project Timeline
Phase	Description	Duration
1	Literature Review & Dataset Selection	Month 1–2
2	Baseline Model Development	Month 3–4
3	NSSM Implementation & Experiments	Month 5–6
4	API Development	Month 7–8
5	Mobile App Integration	Month 9–10
6	Evaluation & Optimisation	Month 11
7	Final Report & Presentation	Month 12
11. Expected Contributions
This project contributes:
Implementation of an entity-aware smoothing mechanism
Comparative experimental analysis
Parameter sensitivity study
Integration into a deployable mobile application
Reproducible GitHub repository
