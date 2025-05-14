# 🚨 Abusive Language Detection using BERT

This project detects abusive comments on social media using **Natural Language Processing (NLP)** and a **BERT-based deep learning model**. It leverages pre-trained transformer embeddings to classify text into multiple categories of abuse with high accuracy.

---

## 🧠 Model Overview

- **Model**: DistilBERT (`distilbert-base-multilingual-cased`)
- **Framework**: PyTorch + HuggingFace Transformers
- **Dataset**: 143,000+ labeled comments (Kaggle Toxic Comment Classification)
- **Output Labels**:
  - `toxic`
  - `severe_toxic`
  - `obscene`
  - `threat`
  - `insult`
  - `identity_hate`

---
## 📥 Dataset

- **Source**: [Kaggle Jigsaw Multilingual Toxic Comment Classification Challenge](https://www.kaggle.com/competitions/jigsaw-multilingual-toxic-comment-classification)

---
## 🔧 Tech Stack

- Python
- PyTorch
- HuggingFace Transformers
- Flask (for web deployment)
- HTML/CSS (frontend)

---
## 🚀 How to Run

1. **Install dependencies**
   ```bash
   pip install flask torch transformers

2. **Run the Flask app**
   ```bash
   python app.py
---
## 🖼 Example

Here is how the app looks when running locally:

![Abusive Language Detection Example](Example.png)

## 📌 Future Work

- Add BiLSTM comparison  
- Host live version online (Render, Replit, Hugging Face Spaces)  
- Improve UX with JavaScript and loading spinner

---
## 📂 Suggested Folder Structure
abusive-language-detection/
│
├── app.py                  # Flask backend using BERT
├── model.pt                # Trained PyTorch model
├── model.py                # Model architecture (DistilBERT + classifier)
├── templates/
│   ├── index.html          # User input form
│   └── result.html         # Classification result display
├── README.md
