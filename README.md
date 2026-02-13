# 🎓 AI-Based Answer Sheet Evaluation System

![Project Banner](https://img.shields.io/badge/Status-Active-success) ![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue) ![License](https://img.shields.io/badge/License-MIT-green)

A state-of-the-art automated evaluation system that leverages **Computer Vision**, **Natural Language Processing (NLP)**, and **Machine Learning** to grade handwritten answer sheets with high accuracy. This system streamlines the grading process for educators and provides instant, detailed feedback to students.

---

## 🚀 Features

-   **📝 Automated Grading**: Instantly evaluates handwritten exams using OCR and NLP models.
-   **🤖 AI-Powered Analysis**: Assesses descriptive answers based on semantic meaning, keywords, and context.
-   **📊 Smart Dashboard**: Comprehensive analytics for teachers to track class performance and student progress.
-   **⚡ Instant Feedback**: Students successfully receive detailed result breakdowns immediately after submission.
-   **🔐 Role-Based Access**: Secure login portals for both **Teachers** and **Students**.
-   **📄 Multi-Format Support**: Handles image uploads and PDF generation for reports.

---

## 🛠️ Tech Stack

-   **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
-   **Backend**: Python (FastAPI & Flask)
-   **Database**: MongoDB
-   **AI/ML**: TensorFlow, PyTorch, NLTK, Google Gemini API, OCR (Tesseract/EasyOCR)
-   **Deployment**: Ready for local and cloud deployment

---

## ⚙️ Installation & Setup

Follow these steps to run the project locally.

### Prerequisites

-   Python 3.8 or higher
-   MongoDB (installed and running locally)
-   Git

### 1. Clone the Repository

```bash
git clone https://github.com/manish1bhardwaj/AI-BASED-EXAM-EVALUTION.git
cd AI-BASED-EXAM-EVALUTION
```

### 2. Backend Setup

Navigate to the backend directory and set up the virtual environment.

```bash
cd backend
python -m venv venv
# Activate Virtual Environment:
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### 3. Environment Configuration

Create a `.env` file in the `backend/` directory with the following content:

```ini
MONGO_URI=mongodb://localhost:27017/
DB_NAME=exam_system
GEMINI_API_KEY=your_api_key_here
```

### 4. Run the Application

**Start Backend Server:**

```bash
# From the backend directory
uvicorn fastapi_app:app --reload --host 127.0.0.1 --port 5000
```

**Start Frontend Server:**

Open a new terminal in the project root (`AI-BASED-EXAM-EVALUTION/`):

```bash
python -m http.server 8080 --bind 127.0.0.1
```

---

## 📖 Usage Guide

1.  **Access the App**: Open your browser and go to `http://127.0.0.1:8080`.
2.  **Teacher Flow**:
    -   Login as Teacher.
    -   Upload an **Answer Key** (PDF/Image) for an exam.
    -   View student submissions and AI-generated grades.
3.  **Student Flow**:
    -   Login as Student.
    -   Upload **Handwritten Answer Sheets**.
    -   Check results and detailed feedback instantly.

---

## 📂 Project Structure

```
AI-BASED-EXAM-EVALUTION/
├── backend/                # FastAPI Application & Logic
│   ├── routes/             # API Endpoints
│   ├── models/             # ML Models & Evaluation Scripts
│   ├── uploads/            # Stored Exam Files
│   ├── database.py         # DB Connection Logic
│   ├── fastapi_app.py      # Main Server File
│   └── requirements.txt    # Python Dependencies
├── css/                    # Frontend Styles
├── js/                     # Frontend Scripts
├── index.html              # Landing Page
├── login.html              # Authentication Page
├── teacher-dashboard.html  # Teacher Interface
├── student-dashboard.html  # Student Interface
└── README.md               # Project Documentation
```

---

## 🤝 Contributing

Contributions are welcome! Please fork the repository and create a pull request for any feature enhancements or bug fixes.

---

## 📞 Contact

For queries or support, please contact:
**Manish Bhardwaj** - [GitHub Profile](https://github.com/manish1bhardwaj)
