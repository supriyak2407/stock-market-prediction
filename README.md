# Stock Price Prediction System 

## Overview

This project aims to create a stock price prediction system by integrating mathematical functions, machine learning algorithms, and external factors to enhance prediction accuracy and support informed investment decisions. The system uses regression and Long Short-Term Memory (LSTM) models separately for predicting stock prices. The dataset is obtained from Yahoo Finance and includes variables such as open, close, low, high, and volume.


## Introduction

Stock prediction is a challenging task, but it becomes more manageable with machine learning. This project utilizes supervised machine learning on a dataset obtained from Yahoo Finance, comprising open, close, low, high, and volume variables. The system is tested on a separate test dataset to evaluate its performance.

## Methodology

### 1. Regression Based Model

#### Regression Based Model 

- Regression is used to predict continuous values by minimizing error through the linear regression algorithm.
- The linear regression equation used is: V = a + bK + error, where V is the continuous value, K represents known independent values, and a, b are coefficients.
- The dataset is processed using the pandas library, and parameters to be predicted (stock prices) are calculated.
- Data is divided into train sets for cross-validation to avoid overfitting, with the test set typically kept at 20% of the entire dataset.
- Linear regression is performed on the data, and predictions are plotted to visualize stock market prices vs. time.

### 2. LSTM Based Model

- LSTM is an advanced version of Recurrent Neural Networks (RNN) with the ability to handle long-term dependencies.
- It addresses the vanishing gradient problem by incorporating a remembering cell, input gate, output gate, and forget gate.
- The sequential model includes two stacked LSTM layers with an output value of 256.
- A dropout value of 0.3 is set to prevent overfitting, and a core dense layer connects neurons to the next layer, producing output.
- The model is compiled with a mean square cost function.

## Result

The LSTM and Regression techniques applied to the Yahoo Finance dataset have demonstrated improved prediction accuracy, yielding positive results for stock price predictions.

## Conclusion

The integration of LSTM and Regression techniques in stock price prediction has shown promising results, affirming the efficacy of machine learning in predicting stock markets more accurately. Future improvements may involve utilizing larger datasets and exploring other machine learning models to enhance accuracy.

## Future Enhancements

- Utilize larger datasets to improve prediction accuracy.
- Explore additional machine learning models for comparative analysis.
- Enhance the system's robustness and adaptability.
