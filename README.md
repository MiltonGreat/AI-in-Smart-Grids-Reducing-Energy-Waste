# Smart Grid Energy Analysis

## Overview

This project analyzes energy consumption data from a smart grid system to identify inefficiencies, detect anomalies (such as power wastage), and predict and prevent such inefficiencies in real time. The goal is to enhance energy efficiency and improve the overall performance of the grid.

### Dataset

The dataset includes various energy-related metrics such as:

- Voltage (V)
- Current (A)
- Power Usage (kW)
- Frequency (Hz)
- Fault Indicator
- Fourier Transform (FFT) values

### Methodology

1. Data Preprocessing
- Cleaned and processed raw energy consumption data.
- Handled missing values and normalized features where necessary.

2. Exploratory Data Analysis (EDA)
- Identified key relationships, including the strong correlation between current and power usage.
- Analyzed voltage and frequency fluctuations.
- Examined Fourier Transform values to study frequency component behavior.

3. Machine Learning Model for Prediction
- Developed a predictive model to detect inefficiencies.
- Achieved high predictive accuracy (R² = 0.996, MAE = 0.019).

4. Classification Model for Energy Efficiency
- Classified grid performance into "Efficient" and "Inefficient" states.
- Identified class imbalance issues where inefficiencies were harder to detect.
- Proposed improvements to enhance model performance on minority class detection.

### Key Findings

- Voltage and Power Usage exhibit moderate variation, indicating normal but stable grid behavior.
- Faults are relatively rare (mean = 0.97), but their occurrence suggests the need for proactive monitoring.
- Current and Power Usage have a strong linear relationship, confirming expected electrical properties.
- Weak correlation between voltage, frequency, and other variables suggests limited interaction in this dataset.
- The model performs exceptionally well in predicting power usage but struggles with detecting inefficiencies due to class imbalance.

### Future Improvements

- Address class imbalance using techniques like SMOTE or class weighting.
- Enhance feature engineering for better inefficiency detection.
- Implement real-time anomaly detection for power quality monitoring.
- Explore deep learning models for improved forecasting accuracy.

### Source

https://www.kaggle.com/datasets/ziya07/smart-grid-monitoring-dataset
