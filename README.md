# Case-3-Task-Quality-Assurance-Machine-Learning-Task
Call Transcript Classification using Machine Learning
📌 Project Overview
This project focuses on using Machine Learning to classify call transcripts into two categories:

Category 6: Introduction Calls
Category 7: Final Loan Details & Next Steps
The goal is to improve recall from 2% (heuristic method) while maintaining high accuracy (~80% or more) for better sales call classification.

📊 Dataset & Preprocessing
Dataset:
400 labeled and 2000 unlabeled examples
Preprocessing Techniques:
Dictionary String Conversion: Structured text format
Feature Engineering:
Low Cardinality Features → One-Hot Encoding
High Cardinality Features → Embedding-based numerical mapping
Label Encoding → Converting categorical target labels to numerical values
Data Splitting → Training, Validation, and Testing sets
🛠 Machine Learning Models Used
Supervised Learning Models
Model	Accuracy (%)	Recall (%)	F1-Score (%)
Random Forest	96.25	96.25	95.60
Gradient Boosting	95.00	95.00	95.48
Decision Tree	92.50	92.50	93.49
✅ Best Performer: Random Forest (Correctly classified 98.75% of labeled data)

Semi-Supervised Learning Model
Category	Accuracy (%)	Recall (%)	F1-Score (%)
Category 6	91.5	100	87
Category 7	91.5	97	97
📌 Techniques Used:

Autoencoder for Feature Extraction
XGBoost Classifier with Pseudo-Labelling
📌 Observation:

Semi-supervised model performed well but struggled with Category 6 due to limited labeled data.
🚀 Key Findings & Observations
✅ Strengths:
✔ Significant improvement over heuristic methods
✔ High recall & F1-score in both categories
✔ Regularization techniques (Gaussian noise, Early Stopping, Dropout) reduced overfitting

⚠ Limitations:
❌ Small labeled dataset (400 examples) → Risk of overfitting
❌ Autoencoder complexity → Did not add significant improvement
