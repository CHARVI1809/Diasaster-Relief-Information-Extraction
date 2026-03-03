# Disaster Relief Information Extraction Using Natural Language Processing and Machine Learning

## Abstract

During natural disasters, social media platforms generate large volumes of real-time textual data. While this data contains potentially critical information for emergency response, a significant portion is noisy or irrelevant. Efficient identification of actionable information is therefore essential.

This study presents a supervised machine learning framework for binary classification of disaster-related tweets into **On-Topic** (relevant) and **Off-Topic** (irrelevant) categories. Traditional Natural Language Processing (NLP) techniques combined with classical machine learning classifiers are evaluated to determine the most effective approach for disaster information filtering.

---

## Research Paper

This repository accompanies the research paper:

**“Disaster Relief Information Extraction Using Natural Language Processing and Machine Learning”**

📁 Available inside the `paper/` directory.

---

## 1. Introduction

Rapid access to reliable information is crucial during disaster response operations. Social media platforms such as Twitter provide immediate, crowd-sourced updates during crises. However, the unstructured and high-volume nature of such data necessitates automated filtering mechanisms.

This project investigates the effectiveness of:

- Classical text preprocessing techniques
- Sparse vector representations (BoW and TF-IDF)
- Multiple supervised classification algorithms

The objective is to determine which model-feature combination achieves the highest classification performance for disaster tweet filtering.

---


## 2. Dataset

- **Dataset:** CrisisLexT6  
- **Total Tweets:** ~60,000  
- **Class Distribution:**
  - On-Topic: 32,462  
  - Off-Topic: 27,420  

The dataset consists of labeled tweets collected during six major disaster events.

⚠️ Due to licensing and privacy constraints, the dataset is not included in this repository.  
Users must download the dataset from the official CrisisLexT6 source and place it inside the `data/` directory.

---

## 3. Methodology

### 3.1 Text Preprocessing

The following preprocessing steps were applied:

- Lowercasing
- Removal of stopwords
- Removal of punctuation and special characters
- Tokenization

These steps reduce noise and improve feature quality.

---

### 3.2 Feature Extraction

Two sparse vector representations were evaluated:

- **Bag of Words (BoW)**
- **Term Frequency – Inverse Document Frequency (TF-IDF)**

Both approaches transform textual data into high-dimensional numerical feature vectors suitable for machine learning classifiers.

---

### 3.3 Classification Algorithms

The following supervised learning models were implemented and evaluated:

- Support Vector Machine (SVM)
- Logistic Regression
- Random Forest
- Naïve Bayes
- Decision Tree
- K-Nearest Neighbors (KNN)

Model performance was compared using accuracy and standard classification metrics.

---

## 4. Experimental Results

### Best Performing Configurations

| Feature Representation | Best Model           | Accuracy |
|------------------------|---------------------|----------|
| Bag of Words           | Logistic Regression | 94.82%   |
| TF-IDF                 | Support Vector Machine | 94.65% |

### Key Findings

- Linear classifiers (SVM and Logistic Regression) performed consistently well.
- Sparse representations are highly effective for short-text classification.
- KNN demonstrated comparatively lower performance due to high-dimensional feature space.
- Classical machine learning approaches remain competitive for binary tweet classification tasks.

Detailed performance metrics and comparative visualizations are available in the `results/` directory.

---

## 5. Project Structure

```
├── notebook/
│ └── Disaster_relief_info_extraction.ipynb
├── data/
├── results/
├── paper/
├── requirements.txt
└── README.md
```
---

## 6. Reproducibility

The experiments presented in this study can be reproduced using the following steps.

### Step 1: Clone the Repository

```bash
git clone https://github.com/CHARVI1809/Disaster-Relief-Information-Extraction.git
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```
 
### Step 3: Run the Notebook
```bash
notebook/Disaster_relief_info_extraction.ipynb
```
---

## 7. Future Work

Future research directions include:

- Integration of deep learning architectures (LSTM, GRU, Transformer-based models)
- Incorporation of contextual embeddings (Word2Vec, GloVe, BERT)
- Real-time streaming tweet classification systems
- Multilingual disaster tweet analysis
- Deployment as an emergency response decision-support system

---
## 8. Authors

**Charvi Gupta**  
B.Tech Computer Science and Engineering  
Manipal University Jaipur  

**Ananya Srivastava**  
B.Tech Computer Science and Engineering  
Manipal University Jaipur  

---
## 9. License

This repository is intended for academic and research purposes only.

---

