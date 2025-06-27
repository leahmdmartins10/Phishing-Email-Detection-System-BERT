# Phishing Email Detection System Using BERT

This project aims to develop a binary classification model using a fine-tuned BERT transformer to detect phishing emails. The model distinguishes between phishing and legitimate emails by leveraging natural language patterns found in email bodies.

## 🚀 Project Overview

Phishing attacks are a significant threat in cybersecurity. Traditional detection methods rely on rule-based filtering, which often fails against sophisticated attacks. By using BERT (Bidirectional Encoder Representations from Transformers), we aim to build a robust detection system capable of understanding contextual nuances in email content.

## ✅ Progress Summary

As of June 26:

- ✅ **Data Acquisition**: Kaggle and CEAS 2008 datasets have been downloaded and loaded into Google Colab.
- ✅ **Preprocessing**:
  - Data was cleaned and merged.
  - Relevant fields (body text, labels, URL counts) were isolated.
- ✅ **Splitting**:
  - Dataset was split into training (70%), validation (15%), and testing (15%) using stratified sampling.
- ✅ **Tokenization**:
  - Used Hugging Face’s `BertTokenizerFast` to tokenize the email body text.
  - Generated attention masks to support BERT’s input requirements.
- ✅ **Tensor Wrapping**:
  - Converted all features (input IDs, attention masks, labels, and URL counts) into PyTorch tensors.
  - Combined into `TensorDataset`s for training, validation, and testing.
- ✅ **Dataset Inspection**:
  - Verified dimensions: Each input is of shape `[512]` after tokenization, indicating consistent max length truncation.
- 🔜 **Next Steps**:
  - Define the BERT-based classification model.
  - Implement training and evaluation loops.
  - Visualize accuracy/loss metrics.
  - Experiment with URL count integration as an auxiliary feature.

## 🧠 Technologies Used

- Python 3.x
- PyTorch
- Hugging Face Transformers (`bert-base-uncased`)
- Google Colab
- Pandas, scikit-learn

## 📁 File Structure

```
ver_2_June_26_Phishing_Email_Detection_System_Using_BERT.ipynb
data/
  ├── CEAS_08.csv
  ├── kaggle_phishing_dataset.csv
```

## 🤖 Goal

To achieve high test accuracy and generalization performance by fine-tuning a pre-trained BERT model on phishing email classification tasks.

## 👥 Team

- Leah Martins
- Asmita Chandra
- Joonseo Park
- Riya Kapoor

---

Let us know if you'd like to add a model architecture diagram, experiment logs, or integrate Colab links!