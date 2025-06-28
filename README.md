# 🩺 AI-Powered Disease Prediction & Doctor Recommendation System

An intelligent healthcare triage assistant that predicts diseases from clinical notes and symptoms, explains the diagnosis, recommends relevant over-the-counter (OTC) medications, and suggests the appropriate type of doctor — built for accessibility in remote or underserved regions.

## 💡 Overview

This project utilizes state-of-the-art Natural Language Processing (NLP) with **BERT** to classify clinical diagnosis notes into probable diseases and provides actionable medical insights to users. It features a FastAPI backend and a clean web-based frontend.

**Key Features:**
- ✅ Accepts clinical diagnosis notes or symptoms from users
- 🧠 Predicts diseases like Stroke, Sepsis, Type 2 Diabetes, etc.
- 📘 Explains the condition in simple terms
- 💊 Suggests relevant OTC medications
- 🩺 Recommends the correct medical specialist (e.g., Cardiologist, Endocrinologist)

---

## 🚀 Tech Stack

| Component        | Technology                     |
|------------------|--------------------------------|
| Language Model    | `bert-base-uncased` (Hugging Face Transformers) |
| Framework         | FastAPI                        |
| Frontend          | HTML, CSS, JS (basic web UI)   |
| Model Training    | Hugging Face `Trainer` API     |
| Deployment        | FastAPI + Uvicorn              |
| Tokenization      | BERT Tokenizer with truncation & padding |

---

## 🧪 Dataset

- **Size:** ~5,000 clinical diagnosis notes
- **Classes:** Stroke, Sepsis, Type 2 Diabetes, etc.
- **Balance:** Each class had ~40–60 samples
- **Source:** Simulated/sanitized for privacy

---

## 🎯 Model Training

- Preprocessing: Text cleaning, tokenization using BERT tokenizer
- Model: Fine-tuned `BertForSequenceClassification`
- Loss Function: Cross-Entropy
- Optimizer: AdamW
- Evaluation Metrics: Accuracy, Precision, Recall, F1-score
- Training Framework: Hugging Face Trainer API
- Achieved 100% performance metrics after careful validation and test-time checks.

---

### Output:
- 🔍 Predicted disease
- 📖 Explanation of the disease
- 💊 OTC medications
- 🩺 Specialist recommendation

---

## 📂 Project Structure

