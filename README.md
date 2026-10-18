# COMP813-Phishing-Email-Detection
Cross-dataset generalisation of NLP models for phishing email detection using Enron and CEAS-08 datasets.
# Cross-Dataset Generalisation of NLP Models for Phishing Email Detection

## Project Overview
This project evaluates the cross-dataset generalisation of three NLP-based email classification approaches: TF-IDF with Logistic Regression, TF-IDF with a linear Support Vector Machine, and a Bidirectional LSTM (BiLSTM).

Models are trained and evaluated using the Enron email dataset, with external evaluation on CEAS-08 to investigate how performance changes under dataset shift.

## Methods
- TF-IDF feature extraction with Logistic Regression
- TF-IDF feature extraction with linear SVM
- BiLSTM text classification
- Unigram and bigram feature comparison
- Cross-dataset evaluation
- Domain-shift, error, sequence-length and robustness analyses

## Repository Structure
- `notebooks/` — experiment and evaluation notebooks
- `results/` — exported metrics and analysis results
- `requirements.txt` — Python dependencies

## Reproducibility
Run the notebooks in numerical order where applicable. Obtain datasets from their authorised sources and configure the dataset paths before execution. Package versions and preprocessing settings should be documented to support reproducibility.

## Authors
- Yug Jain
- Yash Arun Bohre
- Mahir Dharmendrakumar Modi

## Dataset and Results
The report describes the experimental setup, evaluation metrics, findings and limitations. Dataset access and redistribution are subject to the relevant dataset terms.
