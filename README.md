# Credit Card Fraud Detection

## Table of Contents
- [Project Overview](#project-overview)
- [Prerequisites](#prerequisites)
- [Data Acquisition](#data-acquisition)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Model Training](#model-training)
- [Results](#results)

## Project Overview
This project implements a machine learning model to detect fraudulent credit card transactions. Using a dataset of credit card transactions, we train a Random Forest Classifier to identify potential fraud cases based on various transaction features.


## Prerequisites
- Python 3.7+
- Jupyter Notebook
- Required Python packages (listed in `requirements.txt`)

## Data Acquisition
The dataset used in this project is the Credit Card Fraud Detection dataset from Kaggle. To obtain the data:

1. Visit [Kaggle's Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
2. Download the `creditcard.csv` file
3. Place the downloaded file in the `data/` directory of this project

## Setup and Installation
1. Clone this repository:
git clone https://github.com/simha-p/Creditcard_Fraud_Analysis.git
cd credit-card-fraud


2. Create a virtual environment:
python -m venv venv
source venv/bin/activate  # On Windows, use venv\Scripts\activate


3. Install the required packages:
pip install -r requirements.txt


## Usage
1. Ensure you have placed the `creditcard.csv` file in the `data/` directory.
2. Open and run the Jupyter notebook:
jupyter notebook notebooks/credit_card_fraud_analysis.ipynb


## Model Training
The project uses a Random Forest Classifier to detect fraudulent transactions. The model is trained on 80% of the data and tested on the remaining 20%. Key steps in the model training process include:

1. Data preprocessing and exploration
2. Feature selection
3. Model training using RandomForestClassifier
4. Model evaluation using various metrics

The trained model is saved as `random_forest_model.pkl` in the `models/` directory.

## Results
The Random Forest Classifier achieves the following performance metrics:
- Accuracy: 99.96%
- Precision: 97.44%
- Recall: 77.55%
- F1-Score: 86.36%
- Matthews Correlation Coefficient: 0.869

A confusion matrix is  generated to visualize the model's performance.

![Screenshot 2024-09-01 114528](https://github.com/user-attachments/assets/5e21560a-c522-45b4-985b-519d3e260000)
