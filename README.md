# Malicious URLs Detection using Machine Learning

## Introduction

In this project, we address the challenge of detecting malicious URLs using lexical features and machine learning algorithms. With the increasing cybersecurity threats such as phishing, malware injections, and website defacement, it has become crucial to develop automated systems to identify and mitigate these threats.

## Problem Statement

The objective of this project is to classify raw URLs into different categories, including benign (safe), phishing, malware, and defacement URLs, using machine learning techniques. We approach this as a multi-class classification problem, where each URL is assigned a label indicating its type of maliciousness.

## Dataset

We use a dataset containing 651,191 labeled URLs, including 428,103 benign URLs, 96,457 defacement URLs, 94,111 phishing URLs, and 32,520 malware URLs. The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/sid321axn/malicious-urls-dataset).

## Project Flow

1. **Feature Engineering**: We extract 22 lexical features from the raw URLs, including presence of IP address, abnormal URL structure, URL length, hostname length, and more.

2. **Model Building**: We train three tree-based ensemble machine learning models, namely Random Forest, XGBoost, and Light GBM, using the lexical features.

3. **Model Evaluation & Comparison**: We evaluate the performance of each model on a test set and compare their accuracy and detection rates for different types of URLs.

4. **Feature Importance Analysis**: We analyze the feature importance of the best-performing model (Random Forest) to identify the top contributing features for detecting malicious URLs.

5. **Model Prediction**: We implement a prediction function using the trained Random Forest model to classify new raw URLs as benign, defacement, phishing, or malware.

## Usage

To replicate the results or use the trained model for prediction, follow these steps:

1. Clone the repository to your local machine.
2. Install the required dependencies specified in the `requirements.txt` file.
3. Run the provided Python scripts to preprocess the data, train the models, and analyze the results.
4. Use the trained Random Forest model for classifying new raw URLs by calling the `get_prediction_from_url(url)` function.


## Conclusion

In conclusion, this project demonstrates how machine learning algorithms can be utilized to detect malicious URLs effectively. By leveraging lexical features extracted from raw URLs and employing tree-based ensemble models, we achieve high accuracy in classifying different types of malicious URLs. The trained Random Forest model can be used for real-time detection and mitigation of cybersecurity threats associated with malicious URLs.

For any inquiries or suggestions, please feel free to contact the project maintainer.
