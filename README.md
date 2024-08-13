# LLM-MODEL-ASSIGNMENT
# TEXT CLASSIFICATION USING BERT MODEL

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Architecture](#model-architecture)
- [Training and Fine-Tuning](#training-and-fine-tuning)
- [Evaluation](#evaluation)
- [Results](#results)

## Overview
The main aim of the project is to implement a text classification model to categorize the TREC data. The model is based on the BERT architecture, which has proven effective in various NLP tasks.

## Dataset
The dataset used in this project is the `TREC-5` dataset from Hugging Face's `datasets` library. The dataset consists of text data with 6 types of lables.

- **Training set**: 5452 Labels
- **Test set**: 500 Labels

## Exploratory Data Analysis (EDA)
The project includes an EDA step to understand the breakdown of labels in the dataset.

## Model Architecture
The model uses a pre-trained BERT model from Hugging Face's `transformers` library. The architecture is as follows:

- **BERT Model**: Extracts contextual embeddings for the input text.
- **Dense Layer**: A fully connected layer that maps the [CLS] token's output from BERT to the emotion categories using a softmax activation function.

## Training and Fine-Tuning
The BERT model is fine-tuned using the following settings:

- **Optimizer**: AdamW with a learning rate of 5e-5
- **Metrics**: Accuracy
- **Epochs**: 3

During training, the model's performance is monitored on the test set to avoid overfitting.

## Evaluation
The model's performance is evaluated on the test set.

- **Test Accuracy**: 96.20%

Confusion matrices and classification reports are also generated to analyze the model's performance across different labels.

## Results
The fine-tuned BERT model shows high accuracy for the given dataset, with consistent performance across training, and test datasets. The model's confusion matrix and classification reports are available in the results section.
