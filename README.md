# 📄 AI-Powered CV Analyzer

An intelligent CV Analyzer built with **Python, Natural Language Processing (NLP), Machine Learning, and Streamlit**.

This project analyzes a candidate's CV against a specific **job description** and provides a **resume-job match score**. It helps identify how well a CV matches the requirements of a job and highlights areas where the candidate's CV may need improvement.

---

## 🎯 Project Objective

The main goal of this project is to make CV evaluation easier and more informative for job seekers.

Instead of manually comparing a CV with a job description, the application processes both documents and analyzes their textual similarity using NLP and Machine Learning techniques.

The analyzer can help a candidate understand:

- How well their CV matches a particular job
- Which skills and keywords are relevant
- Where their CV may be missing important information
- Whether their resume content is aligned with the job description

This makes the CV more targeted and can help candidates improve their chances of getting noticed during the hiring process.

---

## 🚀 Key Features

### 📤 CV Upload

Users can upload their CV/resume through the Streamlit interface.

The application supports resume text extraction from supported document formats such as:

- PDF
- DOCX

### 📝 Job Description Analysis

The user can provide a job description containing the skills, qualifications, experience, and requirements for a particular position.

### 🧹 NLP Text Processing

The application preprocesses the CV and job description before analysis.

The preprocessing pipeline includes techniques such as:

- Text cleaning
- Tokenization
- Stopword removal
- Lemmatization
- Text normalization

### 🔎 TF-IDF Based Analysis

The project uses **TF-IDF (Term Frequency–Inverse Document Frequency)** to convert text into numerical representations.

This allows the system to identify and compare important words and terms between the CV and job description.

### 🤖 Machine Learning Resume Scoring

A trained Machine Learning model is used to generate a resume-job matching score based on the processed text.

### 📊 Match Score

The application provides a score indicating how closely the CV matches the provided job description.

A higher score generally means that the CV contains more relevant information related to the job requirements.

### 💡 CV Improvement Insights

The analyzer can help candidates identify areas where their CV may not sufficiently match the job description, allowing them to improve their resume before applying.

---

## 🧠 How It Works

The application follows this general workflow:

```text
        CV / Resume
             │
             ▼
      Text Extraction
             │
             ▼
       Text Cleaning
             │
             ▼
      NLP Processing
             │
             ▼
        TF-IDF Vectorization
             │
             ▼
     Machine Learning Model
             │
             │
Job Description ───────────┘
             │
             ▼
      Match Score
             │
             ▼
     CV Analysis Results
