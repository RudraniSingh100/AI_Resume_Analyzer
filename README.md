# AI Resume Analyzer with ATS Match Scoring

A web-based AI application that evaluates resumes against job descriptions and produces an **ATS-style Resume Match Score**, helping candidates understand how well their resume aligns with a specific role.

The system uses NLP and transformer-based semantic similarity to simulate how modern Applicant Tracking Systems (ATS) screen resumes.

---

## 🔍 What This Project Does

- Accepts resumes in **PDF or DOCX** format
- Parses resume content into structured sections
- Compares resume data with job requirements
- Calculates a **Resume Match Score (0–100%)**
- Provides section-wise insights and improvement suggestions

This tool is designed to bridge the gap between job seekers and automated resume screening systems.

---

## 🧠 Core Analysis Logic

The resume evaluation is based on multiple weighted factors:

- **Skill similarity** using transformer embeddings  
- **Experience relevance** against job expectations  
- **Education alignment**  
- **Keyword/entity overlap**  
- **Resume structure completeness** (Skills, Experience, Education, Projects)

All components contribute to a final **ATS-style match percentage**.

---

## 📊 Output Overview

After submission, the application displays:
- Resume Match Score (percentage)
- Individual scores for skills, experience, and education
- Detected and missing resume sections
- Actionable feedback to improve resume quality

---

## 🛠️ Technology Stack

**Frontend**
- HTML, CSS, JavaScript

**Backend**
- Python, Flask
- Flask-WTF

**AI / NLP**
- Transformers (DistilBERT)
- PyTorch
- scikit-learn
- spaCy

**Document Processing**
- PyPDF2
- python-docx

---

## ⚙️ How to Run Locally

### Step 1: Clone Repository
```bash
git clone https://github.com/rudranisingh100/AI_Resume_Analyzer.git
cd AI_Resume_Analyzer

Step 2: Create Virtual Environment
python -m venv venv
source venv/bin/activate

Step 3: Install Requirements
pip install -r requirements.txt

Step 4: Download NLP Model
python -m spacy download en_core_web_sm

Step 5: Start the Application
python run.py

📁 Project Structure
AI_Resume_Analyzer/
├── app/
│   ├── main/
│   │   ├── routes.py
│   │   ├── forms.py
│   │   ├── templates/
│   │   └── static/
├── models/
│   ├── resume_parser.py
│   ├── job_description_parser.py
│   └── resume_scorer.py
├── requirements.txt
├── README.md
└── run.py

🚀 Enhancements Implemented

Introduced explicit ATS-style Resume Match Score

Improved semantic similarity using transformer embeddings

Added resume structure validation

Enhanced feedback generation for missing sections

Cleaner and more interpretable scoring output

🔮 Future Scope

Resume comparison across multiple jobs

User authentication and score history

Cloud deployment (AWS / Azure)

Downloadable resume analysis reports

Fine-tuned NLP models for domain-specific roles

📄 License

This project is licensed under the MIT License.

🧾 Acknowledgement

This project was inspired by open-source ideas and significantly customized with enhanced scoring logic, improved analysis flow, and ATS-oriented evaluation.