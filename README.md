# Gender Prediction from Name using NLP

## 📌 Project Overview

This project focuses on **Natural Language Processing (NLP)** techniques to predict gender based on a person’s **first name**. Gender prediction from names is a common task in applications such as:

* Customer profiling
* Chatbot personalization
* Demographic analytics
* Social research

The project compares approaches using **NLTK**, **SpaCy**, and **Scikit-learn’s Naive Bayes Classifier** to evaluate their effectiveness on name-based gender prediction tasks.

---

## 📂 Dataset

* **NLTK Names Corpus**: Contains male and female names in English.
* **Custom Indian Names Dataset**: Added manually to improve cultural representation.
* Each entry is labeled as **male** or **female**.
* Example structure:

```python
[("Akanksha", "female"), ("Ravi", "male"), ("Sneha", "female"), ("Amit", "male")]
```

---

## ⚙️ Features Extracted

The model extracts **linguistic features** from names, including:

* Last letter of the name
* Last two letters
* First letter
* Name length
* Case-insensitive handling

These features help capture patterns that differentiate male and female names.

---

## 🏗️ Methodology

1. **Preprocessing**

   * Clean and normalize names
   * Add Indian names for diversity
   * Feature extraction using linguistic rules

2. **Models Used**

   * **Naive Bayes Classifier (NLTK)**
   * **Naive Bayes Classifier (Scikit-learn with DictVectorizer)**
   * **SpaCy model for predictions**

3. **Evaluation Metrics**

   * Accuracy Score
   * Observations on ambiguous/unseen names

---

## 📊 Results

* **NLTK Naive Bayes Classifier:** \~80.32% accuracy
* **Scikit-learn Naive Bayes Classifier:** \~80.75% accuracy
* **SpaCy Predictions:** Effective, but dependent on pre-trained linguistic rules

🔹 **Observations**:

* Last letters like `"na"`, `"la"`, `"ld"`, `"us"` strongly influence predictions.
* Both models performed consistently with less than **0.5% accuracy difference**.
* Robust to case variations (e.g., `"mukesh"` vs. `"MUKESH"`).
* Performance drops for ambiguous names (e.g., `"Kiran"`, `"Robin"`).

---

## 🚀 Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/your-username/gender-prediction-nlp.git
cd gender-prediction-nlp
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Download NLTK Names Corpus

```python
import nltk
nltk.download("names")
```

---

## 🔍 How to Run

Run the Jupyter notebook:

```bash
jupyter notebook "Gender Prediction from Name Using NLP.ipynb"
```

Steps inside notebook:

* Import libraries
* Load dataset
* Extract features
* Train classifiers
* Evaluate models
* Test with custom names

---

## 📌 Future Improvements

* Extend dataset with **global names** for better generalization
* Explore advanced NLP models (**RNN, LSTM, BERT**)
* Deploy as a **Flask/Streamlit web app** for real-time prediction

---

## 🤝 Contributing

Contributions are welcome! You can improve datasets, models, or deploy the project.

---

## 📧 Contact

👩‍💻 **Akanksha Sawant**

* 📍 Pune, India
* 💼 [LinkedIn](https://www.linkedin.com/in/akanksha-sawant-29260226a/)
* 🖥️ [GitHub](https://github.com/AkankshaASawant)

---
