# 🎯 Employee Skill Gap Analyser & Learning Path Generator

An AI-powered HR tool that evaluates employee skills against target roles, identifies proficiency gaps, and generates tailored 6-month learning paths using Udemy course recommendations and the Groq LLM (Llama 3).

## 🌟 Key Features

- **📊 Skill Gap Matrix:** Maps current employee skills against role requirements (inspired by the O*NET database) to identify met, partial, or missing skills.
- **🧠 AI Career Insights:** Leverages Groq's `llama-3.3-70b-versatile` model to provide professional, encouraging, and practical advice on bridging major skill gaps.
- **📚 Course Recommendations:** Analyzes a dataset of Udemy courses to recommend highly-rated and relevant learning resources tailored to the specific missing skills.
- **🗺️ Personalized Learning Path:** Automatically generates a comprehensive, month-by-month, 6-month learning roadmap tailored to the employee's target role.
- **📥 DOCX Report Export:** Compiles the gap analysis, course recommendations, and learning path into a downloadable, professional Word document.
- **🎨 Interactive UI:** Beautiful, dynamic, and easy-to-use Streamlit web application.

## 🛠️ Technology Stack

- **Frontend:** Streamlit, Custom CSS
- **Backend/Logic:** Python, Pandas
- **AI/LLM:** Groq API (Llama-3.3-70b-versatile)
- **Data:** Udemy Courses Dataset, O*NET-inspired Role Definitions
- **Document Generation:** `python-docx` (for Word reports) and `python-pptx` (for PowerPoint generation)

## 📂 Project Structure

```text
D11_SkillGapAnalyser/
├── app.py                   # Main Streamlit application entry point
├── gap_analyser.py          # Core logic for skill mapping and gap matrix computation
├── course_recommender.py    # Logic for finding matching Udemy courses based on gaps
├── llm_handler.py           # Integration with Groq API for insights and learning paths
├── docx_exporter.py         # Handles generation of downloadable Word reports
├── generate_ppt.py          # Script for automating PPT presentation generation
├── architecture.png         # System architecture diagram
└── data/
    └── udemy_courses.csv    # Dataset used for course recommendations
```

## 🚀 Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/skill-gap-analyser.git
   cd skill-gap-analyser
   ```

2. **Create a virtual environment (Optional but recommended):**
   ```bash
   python -m venv venv
   # On Windows use:
   venv\Scripts\activate
   # On Mac/Linux use:
   source venv/bin/activate
   ```

3. **Install dependencies:**
   Make sure you have the required packages installed. 
   ```bash
   pip install streamlit pandas groq python-docx python-pptx
   ```
   *(Note: You can also generate a `requirements.txt` file and run `pip install -r requirements.txt`)*

4. **Run the application:**
   ```bash
   streamlit run app.py
   ```

## 💡 Usage Guide

1. **Configure API:** Obtain an API key from [console.groq.com](https://console.groq.com/) and enter it in the sidebar configuration section.
2. **Employee Input:** Enter employee details (name, experience, current role), their current skills with proficiency levels, and the target role they wish to transition to.
3. **Analyze Gaps:** Click on the "Analyse Skill Gaps" button to view a visual and detailed matrix of where the employee stands.
4. **Generate Learning Path:** Switch to the "Learning Path" tab to get course recommendations and prompt the AI to build a 6-month roadmap.
5. **Export:** Go to the "Export Report" tab to download the findings and roadmap as a professional DOCX file.

## 🤝 Contributors
Domain 11 — HR & Workforce AI
- Maitri
- Ria
- Sagar
- Puneet
