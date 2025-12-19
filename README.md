# COSE36203 Term Project Repository

This repository contains my implementation of the YouTube video category classification model using TF-IDF and an improved Multilingual BERT approach.  
It includes the final code, dataset, and experiment results used for the team project.

## How to Run
1. Open the code in Google Colab  
2. Upload the dataset (youtube_videos_big.csv)  
3. Run all cells from top to bottom  
## Model Overview
- Baseline: TF-IDF + Logistic Regression  
- Improved Model: Multilingual BERT with oversampling  
## Dataset Description
The dataset contains YouTube video metadata including title, description, tags, and category ID.  
After preprocessing and mapping, a total of 11 category groups were used for classification.
## Running Environment
This code is designed to run in Google Colab using GPU.
Required libraries:
- transformers
- datasets
- scikit-learn
- imbalanced-learn
  
## Team Integration
This classifier is used as the category prediction component in our full project pipeline.
It connects with:
- Sentiment Analysis Module
- LLM-based Final Report Generator
  
## Project Purpose
This project aims to build an automatic YouTube video category classifier as part of a larger
team system that includes sentiment analysis and LLM-based report generation.
## Model Performance Summary
- TF-IDF Baseline Accuracy: ~0.58  
  - Strong performance on short text (title, tags)  
  - Limited performance on minority classes  
## Improved Multilingual BERT Accuracy: ~0.57  
  - Significant improvement from initial 0.49 accuracy  
  - Better recall for minority categories due to oversampling  
