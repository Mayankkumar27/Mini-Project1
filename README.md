Mini-Project-2: Introduction to LLMs & Generative AI

📊 Sentiment Analysis using NLP & Word Embeddings

📌 Project Overview

This project is developed as part of Mini Project 2 – Fundamentals of NLP: Text Cleaning & Vectorization in the course Introduction to Large Language Models and Generative AI.

The objective is to create an automated sentiment analysis pipeline for e-commerce product reviews. The system categorizes customer feedback into Positive, Negative, or Neutral sentiments.
It highlights the role of text preprocessing, vectorization techniques (BoW, Word2Vec, GloVe), and dataset preparation for downstream machine learning tasks.

⸻

🚀 Problem Statement

An e-commerce platform specializing in electronic gadgets is experiencing:
	•	A 200% increase in its customer base over the past three years
	•	A 25% rise in feedback volume

Manually analyzing thousands of reviews has become infeasible.
The absence of an automated system can lead to:
	•	Higher customer churn
	•	Damage to brand reputation
	•	Potential financial setbacks

To address this, the company requires an AI-based sentiment classification solution.

⸻

📂 Dataset Details
	•	Product ID → Unique product identifier
	•	Review Text → Customer feedback/comments
	•	Sentiment Label → Positive / Negative / Neutral
	•	Dataset Size → 1007 rows × 3 columns

⸻

🛠️ Methodology

🔹 1. Text Preprocessing
	•	Removal of punctuation & special symbols
	•	Conversion of text to lowercase
	•	Stripping redundant whitespaces
	•	Stopword removal using NLTK
	•	Stemming (Porter Stemmer)
	•	Lemmatization (WordNet Lemmatizer)

🔹 2. Exploratory Data Analysis (EDA)
	•	Visualization of sentiment distribution (class imbalance observed)
	•	Word frequency plots to capture common patterns

🔹 3. Feature Engineering & Vectorization
	•	Bag of Words (BoW) representation
	•	Word2Vec embeddings (CBOW & Skip-gram)
	•	GloVe embeddings for semantic context

🔹 4. Model Evaluation Metrics
	•	Macro F1-Score (handles imbalance better than accuracy)
	•	Precision, Recall per sentiment class
	•	Confusion Matrix for error analysis

⸻

📈 Key Findings
	•	Dataset is imbalanced, with ~85% reviews labeled as Positive.
	•	Macro F1-Score provides a more reliable metric than accuracy.
	•	Word embeddings (Word2Vec, GloVe) outperform BoW in capturing semantic relationships.

⸻

🏗️ Technology Stack
	•	Python → Pandas, NumPy, Scikit-learn
	•	NLTK & Gensim → Preprocessing and embeddings
	•	Matplotlib & Seaborn → Data visualization
	•	Google Colab → Development & execution environment

⸻

📊 Workflow

flowchart TD
    A[Raw Review Data] --> B[Text Preprocessing]
    B --> C[EDA & Visualization]
    C --> D[Vectorization Techniques]
    D --> E[Embeddings: Word2Vec & GloVe]
    E --> F[Model Training & Evaluation]
    F --> G[Future Scope: Deployment]

