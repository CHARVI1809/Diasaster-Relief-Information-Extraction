🌍 Disaster Relief Information Extraction using NLP
📌 Overview

During natural disasters, social media platforms like Twitter generate massive amounts of real-time information. However, not all tweets are relevant for emergency response.

This project focuses on binary classification of disaster-related tweets into:

On-Topic (relevant disaster information)

Off-Topic (irrelevant content)

The system applies Natural Language Processing (NLP) and Machine Learning (ML) techniques to automatically filter useful disaster information, supporting faster and more effective relief efforts.

📄 Research Paper

This repository accompanies the research paper:

“Disaster Relief Information Extraction Using Natural Language Processing and Machine Learning”

📁 Available in the paper/ directory.

📂 Dataset

Dataset: CrisisLexT6

Size: 60,000 tweets

Classes:

On-Topic: 32,462

Off-Topic: 27,420

⚠️ Due to privacy and licensing restrictions, the dataset is not included in this repository.
Please download it from the original CrisisLexT6 source and place it in the data/ directory.

🛠️ Methodology
🔹 Text Preprocessing

Lowercasing

Stopword removal

Punctuation & special character removal

Tokenization

🔹 Feature Extraction

Bag of Words (BoW)

Term Frequency–Inverse Document Frequency (TF-IDF)

🔹 Machine Learning Models

Support Vector Machine (SVM)

Random Forest

Logistic Regression

Naïve Bayes

K-Nearest Neighbors (KNN)

Decision Tree

📊 Results Summary
🔸 Best Performing Models

BoW: Logistic Regression (94.82%)

TF-IDF: SVM (94.65%)

SVM, Random Forest, and Logistic Regression consistently outperformed other classifiers, while KNN showed lower performance due to high-dimensional text data.

Detailed metrics and comparison plots are available in the results/ directory.

📁 Project Structure
├── notebook/
├── data/
├── results/
├── paper/
├── requirements.txt
├── README.md

⚙️ How to Run

Install dependencies

pip install -r requirements.txt


Open the notebook

jupyter notebook


Run all cells in Disaster_relief_info_extraction.ipynb

🔮 Future Scope

Deep learning models (LSTM, BERT)

Real-time tweet classification

Multilingual disaster data

Deployment as a web-based system

👩‍💻 Authors

📍Charvi Gupta
  B.Tech CSE, Manipal University Jaipur

📍Ananya Srivastava
  B.Tech CSE, Manipal University Jaipur


📜 License

This project is for academic and research purposes.
