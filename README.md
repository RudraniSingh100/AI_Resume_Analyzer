# AI Resume Analyzer with ATS Match Scoring

An AI-powered web application that analyzes resumes against job descriptions and generates an **ATS-style Resume Match Score**, helping candidates understand how well their resume aligns with a specific role.

The system uses **NLP and transformer-based semantic similarity** to simulate how modern Applicant Tracking Systems (ATS) screen resumes.

---

## 🚀 Getting Started

### 1️⃣ Prerequisites
Make sure you have the following installed:
- Python 3.8 or higher
- pip (comes with Python)
- Git

---

### 2️⃣ Clone the Repository
```sh
git clone https://github.com/rudranisingh100/AI_Resume_Analyzer.git
cd AI_Resume_Analyzer
```

---

### 3️⃣ Create a Virtual Environment
```sh
python -m venv venv
```

Activate it:

**Linux / macOS**
```sh
source venv/bin/activate
```

**Windows**
```sh
venv\Scripts\activate
```

---

### 4️⃣ Install Dependencies
```sh
pip install -r requirements.txt
```

---

### 5️⃣ Download spaCy Language Model
```sh
python -m spacy download en_core_web_sm
```

---

### 6️⃣ Run the Application
```sh
python run.py
```

Open your browser:
```
http://127.0.0.1:5000/
```

---

## 🔍 Features
- Upload resumes in **PDF or DOCX**
- Resume parsing into structured sections
- Job description comparison
- **ATS-style Resume Match Score (0–100%)**
- Section-wise scoring
- Missing section detection
- Resume improvement suggestions

---

## 🧠 How It Works
The analysis is based on:
- Skill similarity using **DistilBERT embeddings**
- Experience relevance
- Education alignment
- Keyword & entity overlap
- Resume structure completeness  
  (Skills, Experience, Education, Projects)

All factors contribute to a final **ATS-style match percentage**.

---

## 📊 Output
- Resume Match Score
- Skills / Experience / Education scores
- Missing sections
- Actionable feedback

---

## 🛠️ Tech Stack

### Frontend
- HTML
- CSS
- JavaScript

### Backend
- Python
- Flask
- Flask-WTF

### AI / NLP
- Transformers (DistilBERT)
- PyTorch
- scikit-learn
- spaCy

### Document Processing
- PyPDF2
- python-docx

---

## 📁 Project Structure
```
AI_Resume_Analyzer/
│-- app/
│   ├── main/
│   │   ├── routes.py
│   │   ├── forms.py
│   │   ├── templates/
│   │   └── static/
│-- models/
│   ├── resume_parser.py
│   ├── job_description_parser.py
│   └── resume_scorer.py
│-- requirements.txt
│-- README.md
│-- run.py
```

---

## 🚀 Enhancements
- Explicit ATS-style scoring
- Transformer-based semantic similarity
- Resume structure validation
- Improved feedback clarity

---

## 🔮 Future Scope
- Multiple job comparisons
- User login & history
- Cloud deployment
- Downloadable reports
- Domain-specific NLP models

---

## 📄 License
MIT License

---

## 🧾 Acknowledgement
Inspired by open-source projects and enhanced with ATS-focused scoring and analysis logic.

---
Happy Coding 🚀
