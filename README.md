# 🔐 Password Strength Analyzer using LSTM Neural Network

This project uses **deep learning (LSTM)** to classify passwords as **Weak**, **Medium**, or **Strong** based on their character patterns. It's built using **TensorFlow**, runs in **Google Colab**, and includes an optional **Gradio UI** for easy testing.

---

## 🚀 Features

- Trainable model using LSTM on character-level password data  
- Uses real password dataset (e.g., RockYou dataset)  
- Assigns strength labels based on structure & entropy rules  
- Saves model and tokenizer for reuse  
- Displays training accuracy graph  
- Supports testing passwords manually or via Gradio interface

---

## 🧠 Model Overview

- Embedding Layer → LSTM Layer → Dense (Softmax)
- Trained using categorical cross-entropy
- Three output classes: Weak, Medium, Strong

---

## 🧪 How to Run in Google Colab

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Upload a CSV file with a `password` column (e.g., `rockyou_cleaned_large.csv`)
3. The model will preprocess data, train, and show accuracy graphs
4. Test passwords using the `test_password()` function

```python
test_password("MyP@ssword123")
