# Airtel-Sentinel AI
Predicting and Prioritizing Telecom Customer Complaints using Machine Learning

Customer support systems in telecom companies process millions of requests daily. However, inefficient complaint handling often results in duplicate agent outreach, unresolved tickets, and increased operational costs.

This project introduces Sentinel AI, an experimental machine learning system designed to analyze customer complaints, detect escalation risks, and estimate operational impact.

The inspiration came from a real-world scenario where a broadband shifting request triggered multiple redundant calls from support agents, even after the issue was resolved. This highlights an opportunity to use AI-driven prioritization and predictive analytics to improve customer support efficiency.

Table of Contents

Project Overview

Problem Statement

Objectives

Key Features

System Architecture

Dataset Overview

Machine Learning Pipeline

Model Details

Customer Rage Meter (Sentiment Analysis)

Dashboard and Visualization

Tech Stack

Installation and Setup

Usage

Example Output

Project Structure

Future Improvements

Business Impact

Contributing

License

Project Overview

Sentinel AI is a machine learning prototype that analyzes telecom customer complaints and predicts which issues are likely to:

Remain unresolved

Escalate

Trigger duplicate customer outreach

Increase operational costs

The system processes complaint text using Natural Language Processing (NLP) and classifies complaints based on resolution probability and customer sentiment.

The goal is to help telecom companies:

Improve customer experience

Reduce operational inefficiencies

Prioritize critical complaints earlier

Optimize support workflows

Problem Statement

Customer support platforms frequently encounter operational inefficiencies such as:

Duplicate outreach from multiple agents

Delayed resolution of complaints

Lack of complaint prioritization

Poor sentiment tracking of customers

Increased operational costs

Without predictive insights, companies rely on reactive support systems rather than proactive complaint management.

Objectives

The primary objectives of this project are:

Build a machine learning model to classify telecom complaints

Predict complaints likely to remain unresolved

Perform sentiment analysis to detect frustrated customers

Estimate the operational cost impact of unresolved tickets

Visualize complaint trends and insights

Key Features
Complaint Text Analysis

Uses NLP techniques to process and extract insights from customer complaints.

Complaint Resolution Prediction

Predicts whether a complaint is likely to be resolved or remain unresolved.

Duplicate Trigger Detection

Identifies patterns that may lead to repeated agent outreach.

Customer Rage Meter

Measures customer sentiment using sentiment analysis techniques.

Operational Cost Estimation

Estimates the potential cost associated with unresolved or escalated tickets.

Data Visualization

Provides insights through visual dashboards.

System Architecture

The workflow of Sentinel AI follows a structured pipeline:

Data Collection

Data Preprocessing

Feature Extraction

Machine Learning Model Training

Sentiment Analysis

Complaint Risk Prediction

Visualization and Reporting

Pipeline Flow:

Customer Complaint → Text Preprocessing → Feature Vectorization → Machine Learning Model → Sentiment Analysis → Insights Dashboard

Dataset Overview

The dataset used in this project simulates telecom customer complaints.

Example Fields
Column	Description
complaint_text	Customer complaint description
issue_type	Type of issue reported
priority	Complaint priority level
resolution_time	Time taken to resolve issue
status	Resolved or unresolved

Example complaint:

"My broadband shifting request is closed but agents keep calling repeatedly."

Machine Learning Pipeline

The machine learning workflow includes the following stages:

1 Data Cleaning

Remove punctuation

Convert text to lowercase

Remove stopwords

2 Text Vectorization

Text data is converted into numerical features using:

TF-IDF Vectorization

3 Model Training

A classification model is trained to predict complaint resolution status.

4 Model Evaluation

Performance is evaluated using:

Accuracy

Precision

Recall

F1 Score

Model Details

Current model implemented:

Naive Bayes Classifier

Reasons for selection:

Effective for text classification tasks

Fast training and prediction

Works well with TF-IDF features

Future models may include:

Logistic Regression

Random Forest

Gradient Boosting

Transformer-based NLP models

Customer Rage Meter (Sentiment Analysis)

Sentiment analysis is used to measure customer frustration levels.

Possible sentiment categories:

Sentiment	Interpretation
Positive	Issue likely minor
Neutral	Informational complaint
Negative	Customer dissatisfaction

Highly negative sentiment complaints can be prioritized for faster resolution.

Dashboard and Visualization

The project includes visualizations for:

Complaint distribution

Sentiment trends

Resolution rates

Estimated operational cost

Libraries used:

Matplotlib

Seaborn

These visualizations help support teams understand customer support trends and bottlenecks.

Tech Stack

Programming Language

Python

Machine Learning

Scikit-learn

Prophet

Natural Language Processing

Sentence Transformers

TF-IDF Vectorizer

Data Processing

Pandas

NumPy

Visualization

Matplotlib

Seaborn

Development Environment

Jupyter Notebook

Installation and Setup

Clone the repository

git clone https://github.com/yourusername/sentinel-ai.git
cd sentinel-ai

Install required dependencies

pip install pandas numpy scikit-learn matplotlib seaborn prophet sentence-transformers

Run the notebook

jupyter notebook Airtel_Sentinel_AI.ipynb
Usage

Load telecom complaint dataset

Run preprocessing pipeline

Train classification model

Perform sentiment analysis

Generate complaint insights and predictions

The system will output predictions regarding:

Complaint resolution likelihood

Customer sentiment

Estimated operational cost impact

Example Output

Example prediction output:

Complaint:
"My request is closed but agents keep calling again and again."

Prediction:

Resolution Risk: High
Sentiment: Negative
Operational Cost Risk: Medium

Suggested Action:

Prioritize ticket review and prevent duplicate agent outreach.

Project Structure
Sentinel-AI
│
├── Airtel_Sentinel_AI.ipynb
├── README.md
├── dataset
│   └── telecom_complaints.csv
├── models
│   └── complaint_classifier.pkl
├── visualizations
│   └── dashboard_images
Future Improvements

Potential enhancements include:

Deep learning based NLP models (BERT)

Real telecom complaint datasets

Real-time complaint monitoring

Deployment using FastAPI or Flask

Integration with customer support platforms

Automated complaint prioritization engine

Business Impact

If deployed in real telecom systems, solutions like Sentinel AI could help:

Reduce duplicate agent calls

Improve customer satisfaction

Prioritize critical complaints

Optimize support workforce allocation

Reduce operational costs

Contributing

Contributions are welcome.

If you would like to improve this project:

Fork the repository

Create a new feature branch

Submit a pull request

License

This project is released under the MIT License.

Author

Hardik Bhardwaj

BTech CSE (Data Science)
Interested in AI, Machine Learning, and Data-driven Product Systems.
