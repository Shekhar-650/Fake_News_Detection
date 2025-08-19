# Fake_News_Detection

Objective
Build a semantic classification model using Word2Vec and supervised learning techniques.
Classify news articles as either true or fake based on their textual meaning, not just syntax.
🧠 Methodology (CRISP-DM Framework)
Business Understanding – Address the challenge of fake news and its impact on public trust.
Data Understanding – Explore True.csv and Fake.csv datasets (21k and 23k samples respectively).
Data Preparation – Clean and merge data, apply POS-based lemmatization, remove punctuation/digits.
Feature Engineering – Generate semantic vectors using a pre-trained Word2Vec (GoogleNews-300) model.
Model Building – Train and evaluate:
Logistic Regression
Decision Tree
Random Forest
Evaluation – Compare models based on Accuracy, Precision, Recall, and F1-Score.
🛠️ Techniques & Tools Used
Language: Python
Libraries: pandas, numpy, spaCy, gensim, matplotlib, seaborn, scikit-learn
Embedding: Word2Vec (GoogleNews-vectors-negative300.bin)
Environment: Jupyter Notebook, Google Colab
Storage: Google Drive for data/model integration
📊 Model Performance
Model	Train Accuracy	Validation Accuracy	Validation Recall
Logistic Regression	86.6%	84.0%	90.5%
Decision Tree	99.7%	74.2%	68.9%
Random Forest	90.4%	77.7%	75.7%
✅ Logistic Regression was the top performer and recommended for deployment.

🔍 Key Insights
Fake news often includes emotionally charged or speculative language.
Word2Vec helped extract meaningful semantic patterns beyond surface-level word matching.
Logistic Regression generalized well and achieved high recall, minimizing false negatives.
