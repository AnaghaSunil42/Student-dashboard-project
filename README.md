AI Student Study Tracker System

The AI Student Study Tracker System is an intelligent data-driven application designed to monitor, analyze, and improve students’ study habits. It enables students to log their study sessions and receive insights based on their performance, while administrators can manage data, monitor system activity, and retrain machine learning models.

This system combines data analytics, machine learning, and interactive dashboards to provide meaningful insights into student behavior, helping users make better learning decisions and improve overall productivity.

Project Structure
project/
├── app.py                        # Authentication + role-based navigation
├── cluster_config.json           # Cluster configuration storage
├── Study_Track_AI_Project.csv    # Main dataset
├── student_logs.csv              # Student session logs
├── users.json                    # Registered users

└── pages/
    ├── 0_Admin_Dashboard.py      # System metrics + retrain model
    ├── 0_Study_Log_Sessions.py   # Student study log entry + history
    ├── 1_Student_Interface.py    # Recommendations + chatbot
    ├── 2_Admin_Panel.py          # Clustering + student management
    └── 3_Analytics_Dashboard.py  # EDA charts + correlation analysis
Key Features
Authentication & Role-Based Access
Secure login system for Students and Admins with controlled navigation.
Study Session Logging
Students can record daily study sessions and track their history.
Admin Dashboard
Displays system metrics such as total sessions, active users, and model performance.
Machine Learning Integration
Uses clustering (K-Means) to analyze student behavior and group performance levels.
Student Recommendations & Chatbot
Provides personalized suggestions and interactive support.
Analytics Dashboard
Includes EDA charts, correlation analysis, and performance visualization.
Technologies Used
Frontend/UI: Streamlit
Backend: Python
Data Handling: Pandas
Visualization: Plotly
Machine Learning: Scikit-learn (K-Means Clustering)
Storage: CSV, JSON
Workflow
User registers and logs in through app.py
Role-based navigation directs users to appropriate dashboards
Students log study sessions via Study_Log_Sessions
Data is stored in CSV files and processed
ML model performs clustering and analysis
Insights are displayed through dashboards and charts
Advantages
Simple and user-friendly interface
Data-driven insights for better study planning
Role-based system for better control
Scalable and modular architecture
Real-time analytics and visualization
Future Enhancements
Deployment on cloud platforms
Advanced ML models for prediction
Mobile app integration
Real-time notifications and reminders
Improved chatbot with NLP capabilities
Conclusion

The AI Student Study Tracker System is a powerful tool that transforms traditional study tracking into an intelligent and interactive experience. By combining analytics, machine learning, and visualization, it helps students improve performance and enables administrators to make informed decisions based on data.
