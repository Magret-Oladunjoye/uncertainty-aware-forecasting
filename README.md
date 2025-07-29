# Uncertainty-Aware Forecasting – MSc Thesis Project

This repository contains the code pipeline for my MSc thesis. The project focuses on developing a forecasting model tailored for olive cultivation, combining deep learning with uncertainty-aware Bayesian methods.

## Project Summary

Climate plays a critical role in olive farming, and accurate weather forecasting can significantly aid planning and yield. This project implements a hybrid forecasting pipeline using GRUs and Bayesian Ensemble Kalman Filters (BEKF) to provide dynamic, real-time predictions with quantified uncertainty.

## Methods Used

- **GRU (Gated Recurrent Units):** For modeling time-series temperature data  
- **Facebook Prophet:** For decomposing the time series temperature data into trend and residual components 
- **Bayesian Ensemble Kalman Filter (BEKF):** For updating GRU weights with real-time data and managing uncertainty  
- **Preprocessing:** Forward/backward filling for missing values, scaling, and regional standardization

## Contents

- 'Msc_Thesis_Code_Pipeline.ipynb' – Full modeling pipeline from preprocessing to evaluation

## Results Highlights

- The hybrid GRU-BEKF model achieved lower MAE and MSE than standalone Prophet models
- Demonstrated strong generalizability across 5 olive-growing regions
- Captured uncertainty using ensemble-based posterior predictions

## Technologies

- Python 3.x  
- 'pandas', 'numpy', 'tensorflow', 'keras', 'scikit-learn', 'prophet', 'matplotlib'

