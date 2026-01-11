
# 📘 COE025 – Natural Language Processing  
## Project 4: French → Turkish Machine Translation



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
3. **mT5-small**  
4. **MBART**  
5. **ByT5**  
6. **MADLAD**

Each model was evaluated in two stages:
- Pre-trained (before fine-tuning)
- Fine-tuned on the TED2020 dataset

---

## 📈 Evaluation Metrics
To measure translation quality, the following metrics were used:
- **BLEU**
- **METEOR**
- **ROUGE-1**
- **ROUGE-2**
- **ROUGE-L**

Higher values indicate better translation performance.

---

## 📊 Results and Analysis

### ✅ Best Performing Model: **ByT5**
- BLEU score improved from **0.10 → 35.35**
- Highest improvements in METEOR and ROUGE scores
- Best overall translation quality

### 🥈 Second Best Model: **MADLAD**
- BLEU improved from **7.74 → 17.29**
- Consistent and balanced improvements across metrics

### 🔎 Other Observations
- **M2M100** showed moderate improvements after fine-tuning  
- **mT5-small** improved but remained weak overall  
- **MBART** achieved smaller gains compared to other models  

---

## 🧠 Final Conclusion
Fine-tuning significantly improves machine translation performance.  
Among all evaluated models, **ByT5** achieved the best results for **French-to-Turkish translation**, making it the most effective model for this task.

This project highlights the importance of model choice and data preparation in multilingual NLP tasks.

---

## 🛠 Tools & Technologies
- Python  
- HuggingFace Transformers  
- PyTorch  
- sacreBLEU  
- rouge-score  

---

## 📎 Additional Notes
- All models were evaluated using the same test set for fair comparison  
- Results are presented using score tables and performance graphs  
- This README summarizes the workflow explained in the project presentation  

---

## 📚 Course Information
- **Course:** COE025 – Natural Language Processing  
- **Semester:** Fall 2025–2026  
- **Project Type:** Group Presentation (P1)

---
