# answer-quality-classifier
A prototype to classify llm-generated answers based on human-labelled groundtruth.

## Overview

This project is part of the SE_14 (AI Basics) module assessment.  
The goal is to build a small machine learning classifier that predicts whether an LLM-generated answer is **good** or **bad** based on a curated dataset of question–answer pairs.

The project demonstrates:

- Basic understanding of supervised machine learning
- Text feature extraction using TF-IDF
- Training and evaluating simple classifiers
- Interpreting results and reflecting on limitations

## Problem

LLM-based systems often require evaluation pipelines to monitor answer quality and detect regressions.  
In this project, I simulate such an evaluation setup: I collected a small dataset of prompts and LLM answers and manually labeled them as `good` or `bad`.  
The classifier is trained to reproduce these quality judgments automatically.

## Area of AI

**Machine Learning** (supervised classification)

## Algorithms & Techniques

- **TF-IDF** vectorization of text (question + answer)
- **Logistic Regression** as a baseline classifier
- **Linear SVM (Support Vector Machine)** as a second, often stronger classifier
- Train/test split and standard evaluation metrics (accuracy, F1-score)

## Repository Structure

```text
  ├─ data/
  │   └─ llm_answer_quality_dataset.csv
  ├─ notebooks/
  │   └─ llm_answer_quality_classifier.ipynb
  └─ README.md