
# Credit Card Default Prediction

This project focuses on predicting credit card default for clients using various machine learning models. The objective is to evaluate different models and recommend the most effective one for accurately forecasting default risk, helping in credit risk management.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Model Performance](#model-performance)
- [Results and Conclusion](#results-and-conclusion)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The project analyzes a dataset of credit card clients in Taiwan, focusing on predicting whether a client will default on their next payment. Various machine learning models are compared, with a recommendation made based on their performance metrics.

## Dataset Information

The dataset contains information on demographic factors, credit data, payment history, and bill statements of credit card clients. It spans from April 2005 to September 2005 and is publicly available from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients).

### Features

- **Demographic Information**: Age, gender, education level, marital status.
- **Credit History**: Amount of given credit, payment status, previous payments.
- **Target Variable**: Default payment (binary classification: 0 for no default, 1 for default).

## Project Structure

```plaintext
├── data
│   └── credit_card_default.csv        # Dataset used in the project
├── notebooks
│   └── Credit_Card_Default_Prediction.ipynb  # Jupyter notebook with code and analysis
├── src
│   ├── data_preprocessing.py          # Data preprocessing scripts
│   ├── model_evaluation.py            # Model evaluation and comparison scripts
│   └── train_model.py                 # Script to train the chosen model
├── images
│   └── eda_visuals.png                # Visualizations used in the analysis
├── README.md                          # Project readme file
└── requirements.txt                   # Required Python packages
```






### Model Performance
The following models were evaluated for predicting credit card default:   
* LGBMClassifier
* RandomForestClassifier
* XGBClassifier
* ExtraTreesClassifier    
The LGBMClassifier showed the highest accuracy (82%) and F1 score (80%) with minimal computational time, making it the recommended model for deployment.

#### Results and Conclusion
The analysis concluded that the LGBMClassifier is the optimal choice for predicting credit card defaults due to its superior performance across multiple metrics. This model is recommended for credit risk management, helping financial institutions minimize potential losses by accurately predicting client defaults.

### Contributing
Contributions are welcome! Please fork this repository and submit a pull request with your changes.
