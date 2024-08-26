# Stock Price Prediction using Radial Basis Function (RBF) Neural Networks

## Project Overview
This project aims to predict stock prices using a Radial Basis Function (RBF) neural network. The RBF model is implemented to capture complex, non-linear relationships in historical stock market data, allowing for accurate forecasting of future prices. The project also compares the performance of the RBF model with a Multilayer Perceptron (MLP) model.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Dependencies](#dependencies)
- [How to Run](#how-to-run)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction
Stock prices are highly volatile and exhibit complex patterns. Predicting these prices requires models that can capture non-linear relationships effectively. RBF neural networks are well-suited for this task due to their ability to respond differently based on the distance from a central point, making them excellent for interpolation and pattern recognition.

## Dataset
The dataset contains various features including:
- AAPL.csv

## Methodology
1. **Data Collection and Preprocessing**:
   - Historical stock price data was collected, cleaned, and preprocessed to handle missing values, remove outliers, and standardize features.
   
2. **Feature Selection and Engineering**:
   - Relevant features were selected, and new features were engineered based on domain knowledge to improve the model's predictive power.
   
3. **Model Development**:
   - The RBF neural network was implemented with an input layer, hidden layers with RBF neurons, and an output layer. Hyperparameters were fine-tuned through cross-validation.
   
4. **Training and Validation**:
   - The model was trained on the training set and validated using a separate validation set to avoid overfitting.

## Model Architecture
- **Input Layer**: Includes various features extracted from the dataset.
- **Hidden Layer**: Comprises neurons with RBF activation functions (e.g., Gaussian, Multiquadric).
- **Output Layer**: Provides the predicted stock prices.

- The model outperformed traditional models like MLP in predicting stock prices, showcasing its ability to generalize well to unseen data.

## Dependencies
- Python 3.x
- NumPy
- Pandas
- Scikit-learn
- TensorFlow/PyTorch (depending on your implementation)
- Matplotlib (for plotting results)


## Results
The RBF model demonstrated strong performance:
- **Training MSE**: 18.909
- **Test MSE**: 47.861
- **Validation MSE**: 31.940
- **Training R²**: 0.9942
- **Test R²**: 0.9927
- **Validation R²**: 0.9927

