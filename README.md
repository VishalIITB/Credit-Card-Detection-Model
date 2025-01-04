# Credit-Card-Fraud-Detection
## Credit Card Fraud Detection using Neural net | Hybrid CNN-LSTM Model
This project involves detecting fraudulent transactions in a highly unbalanced dataset using a hybrid Convolutional Neural Network (CNN) and Long Short-Term Memory (LSTM) model enhanced with an attention mechanism.

# Dataset
The dataset used for this project is collected from European cardholder data of September 2023. It consists of 284,807 transactions that occurred in 2 days, out of which 492 are labeled as Fraud. This means that the dataset is highly unbalanced with only 0.172% accounting for the Fraud transactions. The dataset contains 31 features, where 28 (V1-V28) are the result of a PCA transformation due to confidentiality issues. The remaining features are:

Time: Seconds elapsed between each transaction and the first transaction in the dataset.
Amount: Transaction amount.
Class: Label of the transaction (1 for Fraud, 0 for Genuine).
# Project Overview
## Goal
The primary objective of this project is to detect fraudulent transactions using a neural network model, specifically focusing on improving the model's performance on an unbalanced dataset.

# Model Architecture
A hybrid CNN-LSTM model with an attention mechanism was developed. This approach leverages the feature extraction capabilities of CNNs and the temporal sequence learning of LSTMs, enhanced by an attention mechanism to focus on important features.

# Techniques and Methods
Data Balancing: Implemented Synthetic Minority Over-sampling Technique (SMOTE) to address the imbalance in the dataset, enhancing the model's performance in detecting fraudulent transactions.
Performance Metrics: The model's performance was evaluated using accuracy and the ROC-AUC score.
Experimental Design
#Algorithm Selection
The research focuses on whether the performance of a hybrid CNN-LSTM model significantly differs with the inclusion of an attention mechanism. The model's parameters were tuned using a combination of GridSearch and Trial-and-Error methods.

# Testable Hypothesis
The hypothesis tested is whether the inclusion of an attention mechanism in the hybrid CNN-LSTM model improves the performance on the Credit-Card Fraud dataset.

Null Hypothesis (H0): The inclusion of the attention mechanism does not significantly improve the model's performance.
Alternate Hypothesis (H1): The inclusion of the attention mechanism significantly improves the model's performance.
If the null hypothesis is accepted, it indicates that the attention mechanism does not provide a significant improvement. If rejected, the alternate hypothesis is accepted, suggesting the attention mechanism significantly enhances the model's performance.

# Results
Accuracy: The model achieved an accuracy of 87% in fraud detection.
ROC-AUC Score: The model demonstrated a high ROC-AUC score of 0.89, indicating its precision in identifying fraud cases.
Conclusion
The hybrid CNN-LSTM model with attention mechanism effectively detects fraudulent transactions in an unbalanced dataset, with significant improvement observed due to the attention mechanism.

#References
[Andrea Dal Pozzolo, Olivier Caelen, Reid A. Johnson and Gianluca Bontempi. Calibrating Probability with Undersampling for Unbalanced Classification. In Symposium on Computational Intelligence and Data Mining (CIDM), IEEE, 2015]
