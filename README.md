# Custom Transformer for Movie Review Sentiment Analysis

A custom Transformer-based binary sentiment classification model (`DemoGPT`) built and trained from scratch in PyTorch on the IMDb movie reviews dataset.

---

> **Academic Note**: This project was completed in partial fulfillment of the requirements for the completion of the course **Future AWS AI Programmer**. It serves as a guided, hands-on implementation to explore custom Transformer architectures, multi-head self-attention mechanics, and PyTorch training workflows from the ground up.

---

## 📌 Project Overview
The objective of this project is to implement a multi-head self-attention Transformer from scratch to classify movie reviews as positive or negative, targeting >75% validation accuracy without relying on pretrained model weights.

### Key Highlights
- **Model Architecture**: Custom `DemoGPT` featuring multi-head self-attention, layer normalization, learned positional embeddings, mean pooling, and a linear classification head.
- **Tokenizer**: Subword tokenization using Hugging Face's `AutoTokenizer` (`bert-base-uncased`).
- **Optimization**: AdamW optimizer with Cross-Entropy Loss and patience-based early stopping.

---

## 📊 Results Summary

| Data | Accuracy | Details |
| :--- | :--- | :--- |
| **Validation (Initial)** | 48.96% | Baseline random performance prior to training |
| **Validation (Best)** | **80.36%** | Achieved at Epoch 5 (exceeds the 75% goal) |
| **Test** | **77.94%** | Evaluated on unseen test reviews |
