# CSE508 Information Retrieval Winter 2024 Assignment-4 Report

**Author:** AKASH KUMAR  
**ID:** MT23012  
**Date of Submission:** 23-04-2024

## Overview
This repository contains the report for Assignment-3 of the CSE508 Information Retrieval course, focusing on fine-tuning the GPT-2 model for generating summaries from Amazon Fine Food Reviews.

## Contents
1. [Data Preprocessing](#1-data-preprocessing)
2. [Methodology](#2-methodology)
3. [Evaluation](#3-evaluation)
4. [Conclusion](#4-conclusion)

## 1. Data Preprocessing
In this section, we preprocess the data in the 'Title' and 'Summary' columns to clean and prepare it for further analysis.

## 2. Methodology
### GPT-2 Setup
Initialize the GPT-2 Tokenizer and Model from Hugging Face using GPT2Tokenizer and GPT2LMHeadModel.
### Data Preparation
Split the dataset into 75% for training and 25% for testing. Develop a custom PyTorch dataset class to preprocess the data, including tokenization and padding.
### Model Fine-Tuning
Fine-tune the pre-trained GPT-2 model on the review dataset to generate summaries. Experiment with different hyperparameters such as learning rate, batch size, and number of epochs.
### Key Parameters
Utilize the following hyperparameters: epoch = 8, learning rate = 5e-5, batch size = 32, sample size = 20000, max length = 180. Train the model on a dataset of 20,000 data points, with an average training time of around 2 hours.
### Query Processing
Implement a function to process queries and present the output in the specified format.

## 3. Evaluation
### ROUGE Score Assessment
Compute ROUGE scores on the test set to evaluate the model's performance. Measure the ROUGE scores for each predicted summary against the corresponding actual summary.
### Analyzing Results
- Quantitative Assessment: Analyze ROUGE scores to assess summarization accuracy.
- Qualitative Evaluation: Review generated summaries for coherence.
- Hyperparameter Influence: Examine how different settings affect model performance.
- Comparison with Other Methods: Compare model's ROUGE scores with simpler methods.

## 4. Conclusion
Summarize findings, highlight model's strengths and weaknesses, and suggest areas for improvement or further research.

