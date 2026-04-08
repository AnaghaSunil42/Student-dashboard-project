# 🎓 AI Student Study Tracking System

An AI-powered student study tracking web application built with Streamlit and KMeans Clustering. The system analyzes student academic behavior and provides personalized study recommendations based on their performance patterns.

---

## 🚀 Features

### 🔐 Authentication
- Role-based login system for Students and Admins
- Secure password hashing with SHA-256
- Register using Student ID or Admin ID

### 🎓 Student Panel
- Personalized study recommendations based on cluster group
- Weekly study schedule and optimal study times
- Study session logging with date, subject, duration, distractions and quiz score
- Study progress visualization over time
- AI Study Assistant chatbot for study related queries

### ⚙️ Admin Panel
- System metrics — active students, study sessions, avg quiz score and dataset size
- CSV dataset upload and management
- Quick Retrain and Full Retrain model retraining options
- Student behavior cluster visualization with scatter plots and radar charts
- Dynamic cluster labeling based on Final Exam Score ranking
- Add new students with automatic cluster assignment
- Analytics dashboard with EDA charts and correlation analysis

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Streamlit | Frontend and UI |
| Scikit-learn | KMeans Clustering and StandardScaler |
| Pandas and NumPy | Data processing |
| Plotly | Interactive charts and visualizations |
| Hashlib SHA-256 | Secure password hashing |
| JSON and CSV | Data storage |

---

## 📁 Project Structure
project/
├── app.py
├── cluster_config.json
├── Study_Track_AI_Project.csv
├── student_logs.csv
├── users.json
└── pages/
├── 0_Admin_Dashboard.py
├── 0_Study_Log_Sessions.py
├── 1_Student_Interface.py
├── 2_Admin_Panel.py
└── 3_Analytics_Dashboard.py
---

## ⚙️ Installation

1. Clone the repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2. Install dependencies
```bash
pip install streamlit pandas numpy scikit-learn plotly
```

3. Run the application
```bash
streamlit run app.py
```

---

## 👤 How to Use

### Student
1. Register using your Student ID from the dataset
2. Login with your Student ID and password
3. View your personalized study recommendations
4. Log your daily study sessions
5. Track your progress over time
6. Ask the AI Study Assistant for study tips

### Admin
1. Register using any Admin ID
2. Login with your Admin ID and password
3. View system metrics and student activity
4. Upload new datasets and retrain the model
5. Add new students and view their cluster assignment
6. Explore analytics and cluster insights

---

## 🤖 ML Model

- Algorithm — KMeans Clustering
- Features — Study Hours per Week, Attendance Percentage, Assignments Completed, Mock Test Score, Final Exam Score
- Normalization — StandardScaler
- Cluster Labels dynamically assigned based on average Final Exam Score ranking

| Rank | Cluster Label |
|---|---|
| 1 | Needs Improvement |
| 2 | Low Engagement |
| 3 | Average Learner |
| 4 | Focused Studier |
| 5 | Consistent Performer |
| 6 | Good Performer |
| 7 | High Achiever |
| 8 | Top Performer |
| 9 | Outstanding Student |
| 10 | Elite Performer |

---

## 📊 Dataset

| Column | Description |
|---|---|
| Student_ID | Unique student identifier |
| Gender | Student gender |
| Age | Student age |
| Study_Hours_per_Week | Weekly study hours |
| Attendance_Percentage | Class attendance percentage |
| Assignments_Completed | Number of assignments completed |
| Previous_Grade | Previous academic grade |
| Internet_Access | Internet availability |
| Mock_Test_Score | Mock test score |
| Final_Exam_Score | Final exam score |
| Performance | Overall performance label |

---

## 📌 Notes

- Make sure Study_Track_AI_Project.csv is present in the root directory before running
- student_logs.csv and users.json are auto created on first run
- cluster_config.json is auto generated when the admin runs the clustering model

---

## 🔮 Future Scope

- Upgrade rule-based chatbot to an LLM powered AI assistant
- Add automated email and SMS performance alerts
- Integrate with real college databases and LMS platforms
- Introduce a parent login module for monitoring student progress
- Explore advanced clustering algorithms like DBSCAN and Hierarchical Clustering
- Develop a mobile friendly version on Streamlit Cloud

---

## 📄 License

This project is for educational purposes.
