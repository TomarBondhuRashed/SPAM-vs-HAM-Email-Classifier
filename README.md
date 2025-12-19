# 📧 SMS Spam Classifier: Natural Language Processing (NLP)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

## 📌 Project Overview
This project is a Natural Language Processing (NLP) application that automatically classifies SMS messages as either **Spam** or **Ham** (Legitimate).

In the modern digital age, filtering unwanted noise is critical. This model uses the **Bag-of-Words** technique to convert human language into machine-readable numerical vectors, achieving a precision rate of >98%.

---

## ⚙️ How It Works (The Logic)
Computers cannot "read" text. They only understand numbers. To solve this, I implemented a 3-step pipeline:

1.  **Text Preprocessing:** Raw messages are cleaned.
2.  **Vectorization (Bag of Words):** Used `CountVectorizer` to create a matrix where every column represents a unique word in the dictionary, and every row represents a message.
3.  **Probabilistic Modeling:** Applied **Multinomial Naive Bayes**, an algorithm based on Bayes' Theorem that calculates the probability of a message being spam given the presence of specific words (e.g., "Free", "Winner", "Urgent").

---

## 📊 Model Performance
* **Algorithm:** Multinomial Naive Bayes (chosen for its superior performance on discrete text counts).
* **Accuracy:** ~98.5%
* **Confusion Matrix:** The model showed exceptional ability to minimize "False Positives" (marking a real message as spam), which is the most critical metric for email filters.

*(Note: Upload your Confusion Matrix image here)*
![Confusion Matrix](images/confusion_matrix.png)

---

## 🧪 "Spam Trap" Test
I manually tested the model with unseen custom messages:
* *"Hey, are we still going for lunch?"* -> **Ham ✅**
* *"Congratulations! You won a $1000 Walmart Gift Card."* -> **Spam 🛑**

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/spam-classifier.git](https://github.com/your-username/spam-classifier.git)
