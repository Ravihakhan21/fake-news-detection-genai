# 📰 Fake News Detection using Transformers

This project applies a pre-trained transformer model (DistilBERT) to detect fake vs real news headlines using only the title text.

## 📘 Overview

- 🔍 **Model**: `distilbert-base-uncased-finetuned-sst-2-english` (Hugging Face)
- 🧠 **Task**: Binary classification — real (0) or fake (1)
- 💻 **Tools**: Python, Hugging Face Transformers, Google Colab, Scikit-learn
- 🗂️ **Data**: Kaggle Fake and Real News Dataset

## 🧪 Results

| Class | Precision | Recall | F1-Score |
|-------|-----------|--------|----------|
| Real  | 0.56      | 0.79   | 0.66     |
| Fake  | 0.57      | 0.31   | 0.41     |
| **Accuracy** |     |        | **0.57**  |

## ⚙️ Methodology

- Used Hugging Face's Transformers pipeline
- Loaded pre-trained sentiment classification model
- Converted output to match fake/real labels
- Evaluated using classification report and confusion matrix

## 🚧 Limitations

- Model fine-tuned on sentiment, not fake news
- Only headlines were used (titles), not full content
- Low recall for fake news due to model-task mismatch

## 🚀 Future Work

- Fine-tune on real fake news datasets (e.g., LIAR)
- Use full news articles for better context
- Add explainability with SHAP or LIME
- Compare performance with RoBERTa, XLM-R, BERT-large

## 👩‍💻 Author

**Raviha Khan**  
BSCS Student | Generative AI Enthusiast 
