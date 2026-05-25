# Aspect-Based Sentiment Analysis of Vietnamese User Reviews in the Fashion Domain

![Python](https://img.shields.io/badge/Python-3.12%2B-blue)
![HuggingFace](https://img.shields.io/badge/Dataset-Hugging_Face-yellow)
![Status](https://img.shields.io/badge/Status-Active-success)

## 📌 Project Overview
This project implements an **Aspect-Based Sentiment Analysis (ABSA)** system tailored for Vietnamese customer reviews in the fashion domain. The goal is to accurately classify customer attitudes (Negative, Neutral, Positive, or Not Mentioned) toward specific product attributes: **Material, Style, Size, Price, and Service**.

## 📊 Dataset
The training data consists of Vietnamese reviews collected from various e-commerce platforms. To optimize the repository size and ensure fast data loading, the dataset is hosted separately on Hugging Face.

🔗 **[View and Download Dataset on Hugging Face](https://huggingface.co/datasets/vinhplaykennen/FashionReviews)**

**Quick Load via Python:**
```python
# pip install datasets
from datasets import load_dataset

dataset = load_dataset("vinhplaykennen/FashionReviews")
print(dataset['train'][:5])
```

## 📂 Folder Structure

```text
Aspect-Based_Sentiment_Analysis/
├── Embedding_Model/          # Contains word embedding models used for text representation (e.g., FastText, CBOW).
│   └── Embedding_CBOW_...
│
├── Preprocessing/            # Contains notebooks for raw data preprocessing, including text cleaning, OCR extraction, and LLM-assisted processing.
│   ├── OCR_TienXuLyVoiLLM.ipynb
│   └── TienXuLyTho.ipynb
│
├── TextClassification_Model/ # Contains various Deep Learning models for the sentiment classification task (e.g., RNN, LSTM, BiLSTM with Attention).
│   ├── FastText_Adv-BiLSTM...
│   ├── FastText_BiLSTM...
│   └── ...
│
├── BaoCao.pptx               # Project presentation slide deck
├── README.md                 # Project documentation
└── requirements.txt          # List of dependencies to install
```

## 🤝 Contributors
- Châu Quốc Vinh
  + [Github](https://github.com/chauquocvinh2234)
  + [Gmail](vinhit220304@gmail.com)
- Vũ Trọng Nghĩa
  + [Github](https://github.com/TrongNghia041104)
  + [Gmail](nghia.hpotaku04@gmail.com)
