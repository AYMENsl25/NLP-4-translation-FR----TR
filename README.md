nlp 4 project translation

# 📘 COE025 – Natural Language Processing  
## Project 4: French → Turkish Machine Translation

---

## 👥 Team Members
- **Aymen Slimani**  
- Tendo  
- Bilal  
- Osama  
- Kasas  

---

## 📌 Project Description
This project is part of the **COE025: Natural Language Processing (Fall 2025–2026)** course.  
The objective of this project is to design, fine-tune, and evaluate **machine translation models** for translating text from **French to Turkish**.

Several **state-of-the-art multilingual NLP models** were tested and compared to observe how **fine-tuning** affects translation quality.

---

## 📂 Dataset Information
- **Dataset Name:** TED2020 v1  
- **Source:** OPUS Open Parallel Corpus  
- **Language Pair:** French (FR) ↔ Turkish (TR)  

### 📊 Dataset Statistics
- 371,600 sentence pairs  
- ~6 million French tokens  
- ~4.5 million Turkish tokens  

The dataset consists of TED talk translations, making it suitable for machine translation tasks.

---

## 🧹 Data Preprocessing
The following preprocessing steps were applied to the dataset:

1. Removal of missing or inconsistent values  
2. Verification of sentence alignment  
3. Tokenization using model-specific tokenizers  
4. Creation of input and target labels  
5. Splitting the dataset into:
   - Training set  
   - Validation set  
   - Test set  

This process ensures proper learning and fair evaluation.

---

## 🔍 Models Implemented
The following models were tested:

1. **M2M100**  
2. **NLLB (French–Turkish)**  
