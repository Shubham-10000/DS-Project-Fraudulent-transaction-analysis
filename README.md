# DS-Project-Fraudulent-transaction-analysis

## overview
This project focuses on detecting fraudulent transactions in a financial dataset simulated for 30 days. The goal is to build a robust machine-learning model that distinguishes between genuine and fraudulent transactions, assisting financial institutions in fraud prevention.

# Fraudulent Transaction Detection

## Data Description
The dataset includes transactional data with the following features:

1. **step**: A unit of time in the simulation, where each step represents 1 hour. The dataset spans 744 steps (30 days).
2. **type**: Type of transaction, including:
   - `CASH-IN`
   - `CASH-OUT`
   - `DEBIT`
   - `PAYMENT`
   - `TRANSFER`
3. **amount**: The transaction amount in local currency.
4. **nameOrig**: The customer initiating the transaction.
5. **oldbalanceOrg**: Initial balance of the customer before the transaction.
6. **newbalanceOrig**: Balance of the customer after the transaction.
7. **nameDest**: The recipient of the transaction.
8. **oldbalanceDest**: The recipient's initial balance before the transaction (not available for merchants).
9. **newbalanceDest**: Balance of the recipient after the transaction (not available for merchants).
10. **isFraud**: Indicates whether the transaction is fraudulent (1: Fraudulent, 0: Genuine). Fraudulent behaviors simulate attempts to transfer or cash out funds illegally.
11. **isFlaggedFraud**: Flags illegal attempts to transfer amounts exceeding $200,000 in a single transaction.

## Objectives
1. Perform **Exploratory Data Analysis (EDA)** to uncover insights and understand patterns in the dataset.
2. Engineer features to improve model performance.
3. Train and evaluate machine learning models for fraud detection.
4. Optimize the models for precision, recall, and overall accuracy.

## Key Features of the Implementation
1. **Data Preprocessing:**
   - Handling missing or incomplete data for merchants.
   - Normalizing and encoding features.
2. **Exploratory Data Analysis:**
   - Visualizing transaction trends and identifying common patterns in fraudulent activities.
3. **Model Development:**
   - Algorithms like Random Forest, Gradient Boosting, and Neural Networks.
   - Testing different feature selection techniques.
4. **Evaluation Metrics:**
   - Precision, Recall, F1 Score, and Confusion Matrix to handle class imbalance effectively.

## Repository Contents
- **Data Dictionary.txt**: Details of all features in the dataset.
- **Jupyter Notebooks**: Include data analysis, feature engineering, and model training processes.
- **Results**: Model performance metrics and visualizations.

## Getting Started
1. Clone this repository.
2. Install dependencies using the requirements.txt file.
3. Load the dataset and explore it using the provided notebooks.
4. Train the models and validate results.

## Technologies Used
- **Languages:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Tools:** Jupyter Notebook

## Future Work
- Integrating advanced fraud detection techniques such as anomaly detection and ensemble models.
- Exploring real-time fraud detection pipelines.
- Deploying the model via APIs for integration with financial systems.

## How to Contribute
Contributions are welcome! Fork the repository, make your changes, and submit a pull request. For feedback or issues, open a discussion in the Issues section.

