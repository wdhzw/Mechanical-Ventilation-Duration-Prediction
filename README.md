# Mechanical Ventilation Duration Prediction using Deep Learning Models

This repository contains the code and data for my FYP project on Mechanical Ventilation Duration Prediction using Deep Learning Models. The project aims to develop a deep learning model that predicts the duration of mechanical ventilation required by a patient using three patient features: Ventilator Reading End-Tidal Carbon Dioxide (ETCO2), Ventilator Reading Respiratory Rate (breaths/min), and Ventilator Reading Tidal Volume (VT) Exhaled.

## Motivation

Mechanical ventilation is a critical treatment for patients with respiratory failure. However, accurately predicting the duration of mechanical ventilation is challenging for clinicians due to the many factors that can affect the duration. In this study, we explore the potential of deep learning techniques to predict the duration of mechanical ventilation for patients in critical care settings.

## Methodology

We used a dataset consisting of 36 patients, some of which had multiple intubations, and carefully preprocessed the data to handle missing values and outliers. We employed Group Shuffle Split to split the dataset into training and validation sets, and a 5-fold cross-validation to evaluate model performance.

We compared four deep learning models (LSTM, CNN, TCN, and GRU) against two baseline models (mean value of the training set and a decision tree regressor). The CNN model demonstrated the best performance in predicting mechanical ventilation duration.

## Results

The CNN model achieved an MAE which is 41% less than the MAE of the mean value baseline. The results suggest the potential of deep learning techniques, particularly convolutional neural networks, for predicting mechanical ventilation duration in critical care settings.

## Usage

To use the code in this repository, follow these steps:

1. Clone the repository to your local machine.
2. Install the required libraries listed in requirements.txt.
3. Run the file in the code file to train and evaluate the models.

## Limitations

The limitations of this study include a small dataset with missing data and some intubations being re-intubations, which may affect the predictions. However, the results demonstrate the potential of deep learning techniques for predicting the duration of mechanical ventilation, and future work could explore the use of larger and more diverse datasets to improve model performance.
