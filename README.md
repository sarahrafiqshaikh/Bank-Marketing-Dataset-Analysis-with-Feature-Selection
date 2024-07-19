# Bank Marketing Dataset Analysis with Feature Selection
 This project analyzes the Bank Marketing dataset from Kaggle using various feature selection techniques to improve model performance.

## Dataset

The "Bank Marketing" dataset from Kaggle contains 20 features and a binary target variable. The goal is to predict if a client will subscribe to a term deposit.

## Project Structure
  - `Bank_Marketing_Dataset_Analysis_with_Feature_Selection.ipynb`: Jupyter notebook containing the full analysis
  - `README.md`: This file, providing an overview of the project
  - `bank_marketing.html`: This file, providing quick overview at glance of the dataset
  - `bank-marketing-dataset`: This file, providing dataset of the project

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- opendatasets
- ydata_profiling

## Installation

```bash
pip install pandas numpy scikit-learn opendatasets ydata_profiling
```

## Usage

1. Clone the repository
2. Run the Jupyter notebook
`Bank_Marketing_Dataset_Analysis_with_Feature_Selection.ipynb`

## Methods

The project explores three feature selection techniques:

1. Correlation-based (Filter method)
2. Recursive Feature Elimination (Wrapper method)
3. Lasso (Embedded method)

These are compared against a baseline model without feature selection.

## Results

### Initial Model (42 features)
- Accuracy: 0.77
- Precision: 0.75 (False), 0.79 (True)
- Recall: 0.83 (False), 0.70 (True)
- F1-score: 0.79 (False), 0.74 (True)

### Correlation-based Selection (24 features)
- Accuracy: 0.78
- Precision: 0.77 (False), 0.78 (True)
- Recall: 0.81 (False), 0.74 (True)
- F1-score: 0.79 (False), 0.76 (True)

### RFE-based Selection (5 features)
- Accuracy: 0.76
- Precision: 0.78 (False), 0.74 (True)
- Recall: 0.75 (False), 0.77 (True)
- F1-score: 0.77 (False), 0.75 (True)

### Lasso-based Selection (24 features)
- Accuracy: 0.81
- Precision: 0.81 (False), 0.80 (True)
- Recall: 0.81 (False), 0.80 (True)
- F1-score: 0.81 (False), 0.80 (True)

## Conclusion

Lasso-based feature selection provided the best overall performance, significantly improving accuracy and achieving balanced predictions across classes. RFE, while slightly decreasing accuracy, drastically reduced the number of features, which could be beneficial for model interpretability and computational efficiency.

## Future Work

- Experiment with other feature selection methods
- Try different machine learning algorithms
- Perform hyperparameter tuning

## Author
Sarah Rafiq Shaikh


