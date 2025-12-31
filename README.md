AI Resume Analyzer with ATS Match Scoring

A web-based AI application that analyzes resumes against job descriptions and generates an ATS-style Resume Match Score, helping candidates understand how closely their resume aligns with a specific role.

The system leverages NLP techniques and transformer-based semantic similarity to simulate how modern Applicant Tracking Systems (ATS) evaluate resumes during the screening process.

🔍 Project Overview

This application enables job seekers to evaluate and optimize their resumes by:

Uploading resumes in PDF or DOCX format

Parsing resume content into structured sections

Comparing resume information with job requirements

Generating a Resume Match Score (0–100%)

Providing section-wise insights and actionable improvement suggestions

The goal is to bridge the gap between candidates and automated resume screening systems used by recruiters.

🧠 Core Analysis Logic

Resume evaluation is performed using multiple weighted components:

Skill similarity using transformer-based embeddings

Experience relevance aligned with job expectations

Education alignment with role requirements

Keyword and entity overlap

Resume structure completeness (Skills, Experience, Education, Projects)

These factors collectively contribute to a final ATS-style match percentage that reflects resume-job alignment.

📊 Output Summary

After analysis, the application provides:

Overall Resume Match Score (percentage)

Individual scores for skills, experience, and education

Identification of detected and missing resume sections

Targeted recommendations to improve resume effectiveness

🛠️ Technology Stack
Frontend

HTML, CSS, JavaScript

Backend

Python

Flask

Flask-WTF

AI / NLP

Transformers (DistilBERT)

PyTorch

scikit-learn

spaCy

Document Processing

PyPDF2

python-docx

⚙️ Running the Application Locally
Step 1: Clone the Repository
git clone https://github.com/rudranisingh100/AI_Resume_Analyzer.git
cd AI_Resume_Analyzer

Step 2: Create and Activate a Virtual Environment
python -m venv venv
source venv/bin/activate

Step 3: Install Dependencies
pip install -r requirements.txt

Step 4: Download spaCy Language Model
python -m spacy download en_core_web_sm

Step 5: Run the Application
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

Explicit ATS-style Resume Match Score

Improved semantic similarity using transformer embeddings

Resume structure validation

Enhanced feedback generation for missing sections

Cleaner, more interpretable scoring output

🔮 Future Scope

Resume comparison across multiple job descriptions

User authentication and score history tracking

Cloud deployment (AWS / Azure)

Downloadable resume analysis reports

Fine-tuned NLP models for domain-specific roles

📄 License

This project is licensed under the MIT License.

🧾 Acknowledgement

This project draws inspiration from open-source initiatives and has been extensively customized with enhanced scoring logic, improved analysis flow, and an ATS-oriented evaluation framework.
