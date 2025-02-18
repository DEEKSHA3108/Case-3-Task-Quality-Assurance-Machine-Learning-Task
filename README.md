# Case-3-Task-Quality-Assurance-Machine-Learning-Task
Call Transcript Classification using Machine Learning
📌 Project Overview
This project applies Machine Learning to classify call transcripts into:

Category 6: Introduction Calls
Category 7: Final Loan Details & Next Steps
Goals
✔ Improve recall from 2% (existing heuristic method)
✔ Maintain high accuracy (~80% or more)
✔ Automate sales call classification

📊 Dataset & Preprocessing
Dataset:

400 labeled examples
2000 unlabeled examples
Preprocessing Steps:

Dictionary String Conversion → Converts dictionary-like text into structured format
Feature Engineering:
Low Cardinality Features → One-Hot Encoding
High Cardinality Features → Embedding-based numerical mapping
Label Encoding → Converts categorical target labels to numerical values
Data Splitting → Training, Validation, and Testing sets
🛠 Machine Learning Models Used
Supervised Learning Models
Random Forest → Best Performer (96.25% Accuracy, 96.25% Recall, 95.60% F1-score)
Gradient Boosting → (95% Accuracy, 95% Recall, 95.48% F1-score)
Decision Tree → (92.5% Accuracy, 92.5% Recall, 93.49% F1-score)
✅ Key Takeaway: Random Forest outperformed all other models, correctly classifying 98.75% of the labeled data.

Semi-Supervised Learning Model
Autoencoder for Feature Extraction
XGBoost Classifier with Pseudo-Labelling
✅ Performance:

Category 6 → 91.5% Accuracy, 100% Recall, 87% F1-score
Category 7 → 91.5% Accuracy, 97% Recall, 97% F1-score
📌 Observation: The semi-supervised model performed well, but struggled with Category 6 due to limited labeled data.

🚀 Key Findings & Observations
✅ Strengths:
✔ Significant improvement over heuristic methods
✔ High recall & F1-score in both categories
✔ Regularization techniques (Gaussian noise, Early Stopping, Dropout) reduced overfitting

⚠ Limitations:
❌ Small labeled dataset (400 examples) → Risk of overfitting
❌ Autoencoder complexity → Did not add significant improvement

🏆 Conclusion
Supervised models (especially Random Forest) outperformed Semi-Supervised models
Substantial accuracy & recall improvement over previous heuristic-based classification
Future improvements could involve increasing labeled data and enhancing feature extraction techniques

Semi-supervised model performed well but struggled with Category 6 due to limited labeled data.
🚀 Key Findings & Observations
✅ Strengths:
✔ Significant improvement over heuristic methods
✔ High recall & F1-score in both categories
✔ Regularization techniques (Gaussian noise, Early Stopping, Dropout) reduced overfitting

⚠ Limitations:
❌ Small labeled dataset (400 examples) → Risk of overfitting
❌ Autoencoder complexity → Did not add significant improvement
