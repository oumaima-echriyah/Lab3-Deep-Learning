# NLP Lab 4: Exploring NLP Language Models

## Objective

This lab focuses on building and evaluating language models for classifying and regressing medical text data in Arabic, emphasizing practical familiarity with NLP techniques.

---

## Part 1: Project Overview

### **Goal**

To collect, preprocess, and analyze medical text data from Arabic sources using recurrent neural network (RNN) architectures. The study emphasizes the classification and regression of the data to understand its relevance to neurology.

---

### **1. Data Collection**

The dataset was sourced from [Webteb](https://www.webteb.com/neurology/diseases), a website providing medical information in Arabic. Using the web scraping library *BeautifulSoup*, we extracted articles and descriptions related to neurological diseases.

---

### **2. Text Scoring**

To determine the relevance of the collected texts, a rule-based scoring system was implemented. This system assigns scores based on the presence of specific medical terms and keywords associated with neurology.

---

### **3. Preprocessing Pipeline**

A comprehensive preprocessing pipeline was created to prepare the text data for analysis and model training. The steps included:  
- **Tokenization**: Breaking text into smaller units.  
- **Stemming and Lemmatization**: Reducing words to their base forms.  
- **Stop Word Removal**: Eliminating irrelevant or common words.  
- **Discretization**: Transforming text into numerical formats for model input.

---

### **4. Model Training**

Four recurrent neural network architectures were employed:  
- **Simple RNN**: Baseline architecture for sequential data.  
- **Bidirectional RNN**: Processes sequences in both forward and backward directions.  
- **GRU (Gated Recurrent Unit)**: An efficient alternative to LSTM, designed to handle vanishing gradients.  
- **LSTM (Long Short-Term Memory)**: Known for its ability to capture long-term dependencies.  

Hyperparameter optimization was conducted to enhance performance across the models.

---

### **5. Model Evaluation**

The models were assessed using the following metrics:  
- **Loss**: Measures the error during training and testing.  
- **Mean Absolute Error (MAE)**: Evaluates regression accuracy.  
- **BLEU Score**: Commonly used for text-related tasks to quantify similarity between predicted and reference texts.

---

### **6. Key Findings**

- The **Bidirectional RNN** outperformed other architectures in terms of accuracy and relevance.  
- While results were promising, further fine-tuning of hyperparameters could enhance performance.  

---

### **Conclusion**

This project successfully demonstrated the potential of deep learning in analyzing Arabic medical text. It highlights the importance of preprocessing and model selection in tackling domain-specific NLP tasks. Future efforts could involve expanding the dataset and incorporating transformer-based architectures like BERT for improved results.
