# 🌴 AI Resume Analyzer 🌴  
*A Tool for Resume Analysis, Predictions, and Recommendations*  

<p align="center">
  <small>Best viewed in <a href="https://github.com/settings/appearance">Light Mode</a> on desktop (recommended)</small>
</p>

![AI-Resume-Analyzer](https://socialify.git.ci/deepakpadhi986/AI-Resume-Analyzer/image?description=1&descriptionEditable=5th%20Sem%20Final%20Year%20Project%20at%20Kirti%20M%20Doongursee%20College%20(2022%20-%2023)&font=Raleway&language=1&pattern=Plus&theme=Light)

<div align="center">
  <!-- Badges -->
  <p>
    <img src="https://img.shields.io/github/last-commit/deepakpadhi986/AI-Resume-Analyzer" alt="last update" />
    <img src="https://badges.frapsoft.com/os/v2/open-source.svg?v=103" alt="open source" />
    <img src="https://img.shields.io/github/languages/top/deepakpadhi986/AI-Resume-Analyzer?color=red" alt="language" />
    <img src="https://img.shields.io/github/languages/code-size/deepakpadhi986/AI-Resume-Analyzer?color=informational" alt="code size" />
    <a href="https://github.com/deepakpadhi986/AI-Resume-Analyzer/blob/main/LICENSE">
      <img src="https://img.shields.io/github/license/deepakpadhi986/AI-Resume-Analyzer.svg?color=yellow" alt="license" />
    </a>
  </p>
  
  <!-- Quick Links -->
  <h4>
    <a href="#preview-">View Demo</a>
    <span> · </span>
    <a href="#setup--installation-">Installation</a>
    <span> · </span>
    <a href="mailto:dnoobnerd@gmail.com?subject=I%20Want%20The%20Project%20Report%20of%20AI-RESUME-ANALYZER%20(2022%20-%2023)&body=Here%20Are%20My%20Details%20%F0%9F%98%89%0D%0A%0D%0AOrganization%2FCollege%20Name%3A%20%0D%0A%0D%0AFull%20Name%3A%20%0D%0A%0D%0AGitHub%20Profile%20%3A%20%0D%0A%0D%0AFrom%20where%20did%20you%20get%20to%20know%20about%20this%20project%3A%0D%0A%0D%0APurpose%20of%20asking%20project%20report%20(describe)%3A%0D%0A%0D%0A%0D%0AIf%20the%20above%20information%20satisfy%20your%20identity%20you%20will%20get%20the%20report%20to%20your%20email.">Project Report</a>
  </h4>
  
  <p>
    <small>
      Built with ❤️ by <a href="https://dnoobnerd.netlify.app/">Deepak Padhi</a> under guidance of <a href="https://www.linkedin.com/in/mrbriit/">Dr. Bright</a>
    </small>
  </p>
  
  <small>
    🚀 Submitted in partial fulfilment for B.Sc CS at <a href="https://kirticollege.edu.in/">Kirti College</a> (2022-23)
  </small>
</div>

<br/>

## 📌 About the Project

<div align="center">
  <img src="https://raw.githubusercontent.com/deepakpadhi986/AI-Resume-Analyzer/main/screenshots/RESUME.png" alt="Project Screenshot" width="600"/>
  
  <p align="justify">
    An intelligent tool that parses resumes using NLP to extract keywords, clusters them into sectors, and provides:
    <ul align="left">
      <li>Personalized recommendations</li>
      <li>Job role predictions</li>
      <li>Detailed analytics</li>
      <li>Resume scoring</li>
    </ul>
    For both applicants and recruiters through keyword matching algorithms.
  </p>
</div>

## 🎯 Scope

- **For Organizations:**
  - Convert resumes into structured tabular data (CSV export)
  - Analyze placement trends and student profiles
  - Track popular job roles and skill demands

- **For Applicants:**
  - Receive actionable improvement suggestions
  - Get predicted suitable job roles
  - Access curated learning resources
  - Test multiple resume versions

<br/>

## 🛠️ Tech Stack

### Frontend
- Streamlit (Primary Interface)
- HTML/CSS/JavaScript (UI Enhancements)

### Backend
- Python (Core Logic)
- Streamlit (Application Framework)

### Database
- MySQL (Data Storage)

### Key Modules
| Module | Purpose |
|--------|---------|
| pandas | Data manipulation |
| pyresparser | Resume parsing |
| pdfminer3 | PDF text extraction |
| Plotly | Data visualization |
| NLTK | Natural language processing |

<br/>

## ✨ Features

### Client Portal
- **Resume Analysis:**
  - Extracts contact info, skills, education
  - Identifies key keywords
  - Calculates experience level
  
- **Recommendations:**
  - Missing skills to add
  - Predicted suitable roles
  - Relevant courses/certifications
  - Interview preparation videos

- **Scoring:**
  - Overall resume quality score
  - Improvement tips

### Admin Portal
- **Data Management:**
  - View all applicant data
  - Export to CSV
  - Access uploaded resumes

- **Analytics Dashboard:**
  - Interactive pie charts for:
    - User ratings
    - Role distribution
    - Experience levels
    - Geographic distribution

### Feedback System
- Rating collection (1-5 scale)
- Comment history
- Visual rating analytics

<br/>

## 🚀 Installation Guide

### Prerequisites
1. [Python 3.9.12](https://www.python.org/downloads/release/python-3912/)
2. [MySQL](https://www.mysql.com/downloads/)
3. [VS Code](https://code.visualstudio.com/Download) (Recommended)
4. [VS Build Tools](https://aka.ms/vs/17/release/vs_BuildTools.exe)

### Setup Steps


# Clone repository
git clone https://github.com/deepakpadhi986/AI-Resume-Analyzer.git
cd AI-Resume-Analyzer

# Create and activate virtual environment
python -m venv venvapp
venvapp\Scripts\activate

# Install dependencies
cd App
pip install -r requirements.txt
python -m spacy download en_core_web_sm

# Database Setup
1. Create MySQL database named 'cv'
2. Update credentials in App.py (Line 95)

# Replace parser file
Copy provided resume_parser.py to:
venvapp\Lib\site-packages\pyresparser\

# Launch application
streamlit run App.py
