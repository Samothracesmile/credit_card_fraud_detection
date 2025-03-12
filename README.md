# credit_card_fraud_detection


# Credit Card Fraud Detection

This repository contains an end-to-end machine learning solution for the [Credit Card Fraud Detection challenge](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) provided by Kaggle. The goal is to accurately identify fraudulent credit card transactions.

## Dataset

The dataset includes anonymized credit card transactions labeled as either legitimate (0) or fraudulent (1). The data is highly imbalanced, with significantly fewer fraudulent cases.

- **Features:** Anonymized PCA components, transaction amount, and transaction time.
- **Target Variable:** `Class` (0 = Legitimate, 1 = Fraudulent).

## Approach

The solution involves:

1. **Data Preprocessing:**
   - Scaling transaction amounts using StandardScaler.
   - Dropping irrelevant or redundant features (e.g., `Time`).

2. **Handling Imbalanced Data:**
   - Implementing Synthetic Minority Over-sampling Technique (SMOTE) to balance the classes.

3. **Model Training:**
   - Random Forest Classifier was chosen due to its robustness against imbalanced datasets and efficiency in identifying complex patterns.

4. **Evaluation Metrics:**
   - Confusion Matrix
   - Classification Report (precision, recall, F1-score)
   - ROC-AUC Score

## Repository Structure

```
credit_card_fraud_detection/
├── data/
│   └── creditcard.csv
├── fraud_detection.py
├── requirements.txt
└── README.md
```

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/credit_card_fraud_detection.git
cd credit_card_fraud_detection
pip install -r requirements.txt
```

## Usage

Run the fraud detection pipeline:

```bash
python fraud_detection.py
```

## Results

The trained model provides detailed metrics for evaluating performance in distinguishing fraudulent transactions.

## Contribution

Feel free to fork, open issues, and contribute improvements through pull requests.
