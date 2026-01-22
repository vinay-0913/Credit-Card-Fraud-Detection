# Credit Card Fraud Detection - README

## Project Overview
This project develops a machine learning model to detect fraudulent credit card transactions using a Random Forest Classifier. The model analyzes historical transaction patterns to distinguish between normal and fraudulent activity, helping financial institutions identify suspicious behavior early.

## Dataset
- **Total Transactions**: 284,807
- **Features**: 31 (Time, V1-V28 anonymized features, Amount, Class)
- **Target Variable**: Class (0 = Normal, 1 = Fraudulent)
- **Class Imbalance**: ~0.17% fraud cases

## Key Steps

1. **Data Loading & Exploration**: Load and analyze transaction data structure
2. **Class Distribution Analysis**: Examine fraud vs. valid transaction ratio
3. **Feature Analysis**: Compare transaction amounts and correlations
4. **Data Preparation**: Split data into 80% training and 20% testing sets
5. **Model Training**: Train Random Forest Classifier on historical data
6. **Model Evaluation**: Assess performance using multiple metrics

## Model Performance

| Metric | Score |
|--------|-------|
| **Accuracy** | 99.96% |
| **Precision** | 98.73% |
| **Recall** | 79.59% |
| **F1-Score** | 88.14% |
| **MCC** | 0.8863 |

## Key Insights
- High precision (98.73%) minimizes false alarms
- Recall of 79.59% indicates some frauds may be missed
- Strong MCC (0.8863) shows balanced predictions despite class imbalance
- F1-score (88.14%) demonstrates good overall model performance

## Requirements
```
numpy
pandas
matplotlib
seaborn
scikit-learn
```

## Installation
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Usage
1. Place `creditcard.csv` in the project directory
2. Open `Online_Payment_Fraud_Detection.ipynb` in Jupyter Notebook
3. Run cells sequentially to train and evaluate the model

## Files
- `Online_Payment_Fraud_Detection.ipynb` - Main notebook with complete analysis
- `creditcard.csv` - Dataset file (required)
