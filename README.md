# Smart Campus Analytics 🎓

### Predict, Optimize & Improve Student Success

**Smart Campus Analytics** is an AI-powered student success platform that helps colleges identify students who may be at academic or placement risk, understand the reasons behind those risks, and recommend timely interventions.

## 🚀 About the Project

Colleges generate large amounts of student data, including attendance, academic performance, Learning Management System (LMS) activity, engagement, technical skills, and placement readiness. However, these details are often analyzed separately.

Smart Campus Analytics combines these indicators into a unified dashboard to help faculty and placement teams make data-driven decisions and support students before their challenges become serious.

## 🎯 Problem Statement

**Smart Campus Analytics: Predict, Optimize & Improve Student Success**

Educational institutions need a better way to:
- Monitor student academic performance.
- Identify students at risk of failing or falling behind.
- Evaluate placement readiness.
- Understand the factors affecting student success.
- Recommend targeted support and improvement activities.

## 💡 Our Solution

The platform integrates student data and calculates an explainable **Student Success Score (0–100)**. It identifies academic and placement risks, displays the reasons behind the predictions, and recommends suitable interventions.

The goal is not to label students, but to help institutions provide timely, personalized support.

## ✨ Key Features

- **Student Success Score:** A score from 0 to 100 based on available student indicators.
- **Academic Risk Detection:** Identifies students who may need academic support.
- **Placement Risk Detection:** Highlights gaps in coding, aptitude, and placement readiness.
- **Interactive Dashboard:** Displays student statistics, score distributions, and risk categories.
- **Explainable Predictions:** Shows the main factors contributing to a risk assessment.
- **Personalized Interventions:** Recommends activities such as coding practice, mentoring, and attendance improvement.
- **Student Segmentation:** Groups students by performance and support needs.
- **Synthetic Dataset:** Enables project demonstrations without using real student records.
- **Data Quality Checks:** Handles duplicate records, missing values, and invalid ranges.

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Frontend | React |
| Backend | Python, FastAPI |
| Data Processing | Pandas, NumPy |
| Visualization | Interactive charts |
| API Testing | FastAPI Swagger UI |
| Data | Synthetic student dataset |
| Testing | Python unit tests |

*Update this table if your actual implementation uses different libraries.*

## 🏗️ System Architecture

```text
Student Data
     |
     v
Data Cleaning & Validation
     |
     v
Unified Student Data
     |
     v
Success Score & Risk Analysis
     |
     v
Recommended Interventions
     |
     v
FastAPI Backend
     |
     v
React Dashboard
     |
     v
Insights for Faculty & Placement Teams
```

## 📊 Data Inputs

The platform can combine the following indicators:

| Data Category | Example Indicators |
|---|---|
| Academics | CGPA, marks, backlogs |
| Attendance | Attendance percentage |
| LMS Activity | Course activity, assignment completion |
| Engagement | Participation, extracurricular involvement |
| Technical Skills | Coding assessment scores |
| Aptitude | Aptitude assessment scores |
| Placement | Interview readiness, placement preparation |
| Feedback | Student feedback and mentoring needs |

## 🧠 How It Works

1. **Collect:** Load student data from the available dataset.
2. **Clean:** Standardize branch names, handle duplicates, and repair invalid values.
3. **Integrate:** Combine academic, attendance, engagement, and placement indicators.
4. **Calculate:** Generate a Student Success Score using a transparent scoring method.
5. **Identify:** Detect academic and placement risk indicators.
6. **Explain:** Display the main factors contributing to each risk assessment.
7. **Recommend:** Suggest appropriate interventions and support activities.
8. **Monitor:** Use the dashboard to review student progress and support needs.

### Example Student Assessment

*Illustrative example only.*

| Indicator | Example Value |
|---|---:|
| CGPA | 5.2 |
| Attendance | 60% |
| Backlogs | 2 |
| Coding Score | 35/100 |
| Aptitude Score | 40/100 |

**Possible insights:**
- Academic support may be needed.
- Attendance improvement may be beneficial.
- Coding practice and aptitude training may improve placement readiness.

The final risk category and score depend on the implemented scoring rules and available data.

## 📁 Project Structure

The following is a suggested structure. Adjust it to match the actual files in your repository.

```text
smart-campus-analytics/
├── backend/
│   ├── app/
│   │   └── main.py
│   └── requirements.txt
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── index.html
├── data/
│   └── synthetic_student_data.csv
├── src/
│   ├── clean_data.py
│   ├── success_score.py
│   └── risk_model.py
├── tests/
│   └── test_smart_campus.py
├── README.md
└── .gitignore
```

## ⚙️ Installation & Setup

### Prerequisites

Install the following:
- Python 3.10 or newer
- Node.js and npm
- Git (optional, for version control)

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd smart-campus-analytics
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

### 2. Set Up the Python Backend

```bash
cd backend
python -m venv .venv
```

Activate the virtual environment.

**Windows:**
```bash
.venv\Scripts\activate
```

**macOS/Linux:**
```bash
source .venv/bin/activate
```

Install dependencies and start the server:

```bash
pip install -r requirements.txt
uvicorn app.main:app --reload
```

The API should be available at:

- API base URL: `http://127.0.0.1:8000`
- Interactive API documentation: `http://127.0.0.1:8000/docs`

### 3. Set Up the React Frontend

Open a new terminal and navigate to the frontend folder:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL printed in your terminal, usually:

`http://localhost:5173`

*Ensure the frontend API URL and backend CORS settings match your local setup.*

## 🧪 Testing

Run the project's unit tests using the command configured for your repository. For a standard Python `unittest` setup, you can use:

```bash
python -m unittest discover -s tests -v
```

Tests should cover:
- Branch-name standardization.
- Duplicate record removal.
- Validation and repair of academic values.
- Success score boundaries.
- Handling missing indicators.
- Academic and placement risk detection.
- Risk explanations and intervention recommendations.

## 🔐 Responsible AI & Privacy

- Use synthetic or authorized data for demonstrations.
- Treat scores as decision-support indicators, not definitive judgments about students.
- Display understandable reasons for risk assessments.
- Avoid using sensitive personal characteristics to make harmful decisions.
- Allow faculty to review recommendations and apply human judgment.
- Protect student data and restrict access to authorized users.
- Evaluate scoring quality and potential bias before real-world deployment.

## 🌱 Future Enhancements

- Secure login for students, faculty, and administrators.
- Database integration for persistent records.
- CSV upload and data validation interface.
- Historical performance trends.
- Intervention tracking and progress monitoring.
- Downloadable PDF and CSV reports.
- More advanced prediction models with proper validation.
- Integration with institutional LMS and placement systems.

## 🏆 Hackathon Impact

Smart Campus Analytics aims to help institutions move from reactive reporting to proactive student support.

**Expected benefits:**
- Earlier identification of students who may need help.
- Better visibility into academic and placement readiness.
- More targeted mentoring and training recommendations.
- Data-driven planning for student success initiatives.

## 👥 Team

**Project:** Smart Campus Analytics  
**Theme:** AI for Education  
**Problem Statement:** Predict, Optimize & Improve Student Success  
**Developed for:** Hackathon Project

Add your team members, institution, and event details here.

## 📄 License

Choose an appropriate license before publishing this project publicly. For example, you may use the MIT License if it suits your team's requirements.

---

**Smart Campus Analytics — Turning Student Data into Actionable Insights.** 🎓
