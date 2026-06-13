# ⚡ SpamShield — AI Email Spam Detection

> **Sukkur IBA University** | Department of Computer Science | AI 6th Semester Final Project | Instructor Dr Ismail Mangrio

A full-stack machine learning web application that classifies emails as **Spam** or **Not Spam** in real time using TF-IDF feature extraction and Logistic Regression.

---

## 🚀 Quick Start

### 1. Prerequisites
- Python **3.10+**
- pip

### 2. Install dependencies

pip install -r requirements.txt


### 3. Train the model *(run once)*


python train_model.py


This will:
- Load and preprocess `emails.csv`
- Train and evaluate the Logistic Regression model
- Save `model/spam_model.pkl` and `model/vectorizer.pkl`
- Save evaluation charts to `static/images/`
- Print accuracy, precision, recall, and F1-score

### 4. Start the web application

python app.py


Open your browser at: **https://6th-semester-ai-project.vercel.app/**



```
spam_detector/
├── app.py                  
├── train_model.py          
├── requirements.txt        
├── README.md               
│
├── data/
│   └── emails.csv          
│
├── model/
│   ├── spam_model.pkl      
│   ├── vectorizer.pkl      
│   └── metrics.json       
│
├── templates/
│   ├── base.html           
│   ├── index.html          
│   ├── analyze.html        
│   ├── dashboard.html      
│   └── about.html          
│
└── static/
    ├── css/main.css        
    ├── js/
    │   ├── main.js         
    │   └── analyze.js      
    └── images/             
        ├── confusion_matrix.png
        ├── metrics_bar.png
        └── class_distribution.png
```




| Step | Details |
|------|---------|
| **Dataset** | 2,000 emails — 1,000 spam / 1,000 ham |
| **Preprocessing** | Lowercase, URL normalisation, digit tokens, punctuation removal |
| **Feature extraction** | TF-IDF vectoriser, unigram + bigram, 5,000 features, sublinear TF |
| **Train/Test split** | 80% train / 20% test (stratified) |
| **Algorithm** | Logistic Regression (C=1.0, L2, max_iter=1000) |
| **Serialisation** | Joblib (model + vectorizer saved as `.pkl`) |


| Metric | Score |
|--------|-------|
| Accuracy  | 100% |
| Precision | 100% |
| Recall    | 100% |
| F1-Score  | 100% |



| Route | Description |
|-------|-------------|
| `/`          | Home page — project intro, stats, feature cards |
| `/analyze`   | Email analyzer — paste email, get instant verdict |
| `/dashboard` | Model dashboard — all metrics, charts, confusion matrix |
| `/about`     | About page — technical details, pipeline, challenges |
| `/api/predict` | REST endpoint (POST JSON `{subject, body}`) |
