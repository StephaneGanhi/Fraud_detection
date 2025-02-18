# Fraud Detection Project

## Overview
This project focuses on detecting fraudulent transactions using a machine learning pipeline. The dataset used contains transaction details, and the goal is to classify transactions as either fraudulent or non-fraudulent.

## Dataset
The dataset used in this project is `fraud_dataset_example.csv`. It contains the following columns:
- `step`: Unit of time (e.g., hour).
- `type`: Type of transaction (e.g., CASH-IN, CASH-OUT, DEBIT, PAYMENT, TRANSFER).
- `amount`: Transaction amount.
- `nameOrig`: Customer who initiated the transaction.
- `oldbalanceOrg`: Balance before the transaction.
- `newbalanceOrig`: Balance after the transaction.
- `nameDest`: Recipient of the transaction.
- `oldbalanceDest`: Recipient's balance before the transaction.
- `newbalanceDest`: Recipient's balance after the transaction.
- `isFraud`: Binary indicator (1 for fraud, 0 for non-fraud).

## Steps
1. **Data Preprocessing**:
   - Loaded the dataset and handled missing values.
   - Encoded categorical variables (e.g., `type`).
   - Created new features (e.g., balance differences).

2. **Model Training**:
   - Split the data into training and testing sets.
   - Trained a Random Forest classifier.
   - Evaluated the model using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.

3. **Visualizations**:
   - Created a bar chart to show the distribution of fraud vs. non-fraud transactions.
   - Exported model metrics for further analysis.

## Results
### Fraud Distribution
![Fraud Distribution](outputs/fraud_distribution.png)

### Model Metrics
| Metric    | Value   |
|-----------|---------|
| Accuracy  | 0.99    |
| Precision | 0.98    |
| Recall    | 0.97    |
| F1-Score  | 0.975   |
| ROC-AUC   | 0.995   |

## How to Reproduce
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/fraud-detection-project.git
