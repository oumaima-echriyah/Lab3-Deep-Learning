
# Lab 3: Deep Neural Network Architecture Using Sequence Models

## **Overview**

The main purpose of this lab is to get familiar with PyTorch and to construct deep neural network architectures for analyzing and processing sequence-based data. The focus is on designing, training, and evaluating various sequence models for tasks involving sequential data.

---

## **Contents**

- [Overview](#overview)  
- [Data Collection](#data-collection)  
- [Preprocessing](#preprocessing)  
- [Model Architectures](#model-architectures)  
- [Evaluation Metrics](#evaluation-metrics)  
- [Results and Insights](#results-and-insights)

---

## **Data Collection**

The dataset was sourced from [Webteb](https://www.webteb.com/neurology/diseases), a platform that provides detailed information on neurological conditions. Relevant data was collected using the BeautifulSoup library for web scraping, with a focus on articles and descriptions in the Arabic language.

---

## **Preprocessing**

A preprocessing pipeline was developed to clean and prepare the sequence data for model training. The steps include:  
- **Tokenization**: Breaking text into smaller meaningful units.  
- **Normalization**: Removing unwanted characters and ensuring consistent formatting.  
- **Stemming and Lemmatization**: Reducing words to their root forms.  
- **Stop Word Removal**: Filtering out common, non-informative elements.  
- **Discretization**: Transforming the text into numerical formats compatible with deep learning models.

---

## **Model Architectures**

Four deep sequence models were implemented and trained:  
1. **Simple RNN**: A baseline architecture for processing sequential data.  
2. **Bidirectional RNN**: Processes sequences in both forward and backward directions to enhance context understanding.  
3. **GRU (Gated Recurrent Unit)**: A lightweight, efficient alternative to LSTM.  
4. **LSTM (Long Short-Term Memory)**: Designed to learn long-term dependencies effectively.

---

## **Evaluation Metrics**

The models were evaluated using the following metrics:  
- **Loss**: Measures the difference between predicted and actual outputs during training.  
- **Mean Absolute Error (MAE)**: Quantifies the average magnitude of prediction errors.  
- **BLEU Score**: Assesses the similarity between model outputs and reference sequences.

---

## **Results and Insights**

- The **Bidirectional RNN** exhibited the best performance, outperforming the other architectures.  
- Hyperparameter tuning significantly influenced model accuracy and overall performance.  
- The preprocessing pipeline ensured high-quality input data, which was critical to achieving good results.

---

## **Conclusion**

This lab successfully demonstrates the use of PyTorch for building and training sequence models to analyze sequential data. The findings underscore the importance of model architecture and preprocessing in achieving effective results. Future enhancements may involve experimenting with larger datasets and exploring transformer-based models.

