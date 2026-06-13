# 📧 SpamShield - AI Email Spam Detection

SpamShield is a Machine Learning web application that detects whether an email is **Spam** or **Not Spam**. It uses Natural Language Processing (NLP), TF-IDF, and Logistic Regression to analyze email text and provide real-time predictions through a simple web interface.

## 🚀 Features

* Detects Spam and Not Spam emails
* Real-time email analysis
* User-friendly web interface
* Machine Learning-based predictions
* Model performance dashboard

## 🛠 Technologies Used

* Python
* Flask
* Scikit-learn
* Pandas
* NumPy
* HTML
* CSS
* JavaScript

## 📦 Installation

Install the required packages:

```bash
pip install -r requirements.txt
```

Train the model:

```bash
python train_model.py
```

Run the application:

```bash
python app.py
```

Open your browser and visit:

```text
http://localhost:5000
```

## 📂 Project Structure

```text
spam_detector/
├── app.py
├── train_model.py
├── requirements.txt
├── README.md
├── data/
├── model/
├── templates/
└── static/
```

## 🧠 How It Works

1. User enters an email.
2. The text is cleaned and processed.
3. TF-IDF converts text into numerical features.
4. The trained Logistic Regression model analyzes the email.
5. The system predicts whether the email is Spam or Not Spam.

## 📊 Machine Learning

* Text Preprocessing
* TF-IDF Feature Extraction
* Logistic Regression
* Accuracy, Precision, Recall, and F1-Score Evaluation

## 🌐 Web Pages

* Home Page
* Email Analyzer
* Dashboard
* About Page

## 👨‍💻 Project Information

**Course:** Artificial Intelligence

**Institution:** Sukkur IBA University

**Semester:** Spring 2026

This project was developed as part of the AI semester project to demonstrate the practical use of Machine Learning and NLP in email spam detection.
