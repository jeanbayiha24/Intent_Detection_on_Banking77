# Banking Intent Classification using Banking77 Dataset

This project implements and compares various NLP techniques for intent classification in banking customer queries using the Banking77 dataset containing 13,083 queries across 77 fine-grained intent categories.

## Key Features

- Implements traditional ML (TF-IDF + Logistic Regression) and deep learning approaches (Sentence Transformers)
- Evaluates few-shot learning performance with SETFIT
- CPU-optimized solutions for resource-constrained environments
- Comprehensive error analysis on banking-specific intents

## Implemented Approaches

### 1. Traditional Machine Learning
- **TF-IDF + Logistic Regression**
- **Word Embeddings (MPNet-v2) + MLPClassifier**

### 2. Few-Shot Learning
- **SETFIT (Sentence Transformer Fine-Tuning)**
  
### 3. DistilGPT-2 based chatbot

## Results Summary

| Model                      | Accuracy | F1-Score |
|----------------------------|----------|----------|
| TF-IDF + Log. Regression   | 0.862    | 0.855    |
| MPNet + Log. Regression    | 0.880     | 0.874    |
| MPNet + MLP                | 0.990    | 0.955    |
| SETFIT (20-shot)           | 0.860    | 0.860    | Generallize better than all the other models

## Installation

1. Clone repository:
```bash
git clone https://github.com/jeanbayiha24/Intent_Detection_on_Banking77.git
cd Intent_Detection_on_Banking77
```

## References
- **Banking77**, https://huggingface.co/datasets/PolyAI/banking77
- **Breaking the Bank with ChatGPT : Few-Shot Text Classification for Finance**, https://arxiv.org/abs/2308.14634
- **Making LLMs Worth Every Penny : Resource-Limited Text Classification in
Banking**, https://arxiv.org/abs/2311.06102
- **Efficient Few-Shot Learning Without Prompts**, https://arxiv.org/abs/2209.11055

## Contributors
- Jean Bayiha
- Chimezie Anthony Odinakachukwu
- Magatte Fall
- Tidiga Aly
