# 💳 Credit Health Coach: Explainable Credit Score Engine

An intelligent mini-project that simulates a user-facing credit health assistant. It analyzes your financial behavior, classifies expenses, predicts credit score movement, and offers **transparent** and **personalized** feedback using **Explainable AI** and **semantic search-based NLP**.

---

## 📌 Introduction

Managing personal credit is confusing and opaque for most users. This project aims to:
- **Demystify credit scores**
- **Classify financial behavior into needs/wants**
- **Predict credit score impact**
- **Explain score changes with SHAP**
- Allow users to **ask questions** like: *"Why did my score drop?"*

All while keeping things **interpretable**, **lightweight**, and **privacy-aware**.

---

## 🧠 Project Overview

We simulate anonymized financial transaction data and credit card usage, then:
- Predict how various spending behaviors impact credit health
- Enable users to upload supporting docs (like credit card bills) using computer vision
- Offer detailed SHAP-based explanations
- Enable semantic, human-like Q&A interaction with a lightweight NLP layer (Level 2)

---

## 📦 Deliverables

### ✅ 1. **Synthetic Data Generator**
- Generate mock data for users’ daily purchases (amount, category, timestamp)
- Tag purchases as needs/wants
- Simulate credit utilization, bill payment patterns, and due dates

### ✅ 2. **Purchase Classifier**
- **Rule-based model** for essential vs non-essential purchases
- Categories: groceries, rent, luxury shopping, bills, travel, etc.

### ✅ 3. **Credit Score Estimator**
- Lightweight ML model (e.g. `XGBoost` or `RandomForest`)
- Trained on synthetic features like:
  - Credit Utilization Ratio
  - Payment History
  - Number of Open Accounts
  - Spending Category Ratios

### ✅ 4. **Explainable AI Layer (⭐ Star Feature)**
- Use **SHAP** to explain individual credit score predictions
- Visual + Textual explanation of what drove score up/down

### ✅ 5. **“My Discussion” NLP Chat Layer (⭐ Star Feature)**
- Use `sentence-transformers` + `FAISS` for **semantic search** of FAQs
- Embed user queries (e.g. *"Why did my score drop?"*)
- Retrieve the closest intent + SHAP-based explanation

### ✅ 6. **Document Understanding Layer**
- Use `Tesseract OCR` or `EasyOCR` to extract info from:
  - Credit card bills
  - ID proofs
- Convert visual data into structured text for model input

---

## ⚙️ Tech Stack

| Layer                | Technology Used                         |
|----------------------|------------------------------------------|
| Programming Language | Python                                   |
| ML Models            | Scikit-Learn, XGBoost                    |
| Explainability       | SHAP                                     |
| NLP                  | SentenceTransformers, FAISS              |
| Semantic Search      | FAISS / Sklearn NearestNeighbors         |
| OCR (CV Layer)       | Tesseract OCR / EasyOCR                  |
| Data Storage         | JSON / Pandas / SQLite (lightweight)     |

---

## 🚀 Features

- 📊 **Spend Classification** — Categorizes daily expenses into needs/wants
- 🔍 **Credit Behavior Simulation** — Models credit health trends
- 🤖 **Credit Score Estimation** — ML-driven score prediction
- 💡 **Explainable AI (SHAP)** — Transparent model decisions
- 💬 **"My Discussion" NLP Interface** — Ask questions and get SHAP-driven answers
- 📷 **Computer Vision Layer** — Extracts structured data from bills/ID docs

---

## 📁 Suggested Folder Structure

