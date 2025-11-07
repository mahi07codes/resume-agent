# RESUME-AGENT: AI-Powered Resume Analysis & Interview Preparation Tool

## Project Overview

RESUME-AGENT leverages artificial intelligence to help job seekers perfect their resumes and prepare for interviews. This application analyzes resumes against job descriptions to provide personalized feedback, improvement suggestions, and interview preparation materials.

## Live Demo

Access the live application: [https://resume-agent-production.up.railway.app/]([(https://resume-agent-967z.onrender.com/)](https://resume-agent-967z.onrender.com/))

## Key Features

- **Resume Analysis**: Evaluate resumes against specific job requirements
- **Skills Gap Identification**: Highlight strengths and areas for improvement
- **Resume Q&A**: Ask questions about your uploaded resume
- **Interview Preparation**: Generate tailored interview questions based on your profile
- **Resume Enhancement**: Receive actionable suggestions to improve your resume


## Setup and Installation

### Prerequisites

- Python 3.8 or higher
- OpenAI API key

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/RESUME-AGENT.git
   cd RESUME-AGENT
   ```

2. **Create and activate a virtual environment**
   ```bash
   # Create virtual environment
   python -m venv venv
   
   # Activate on Windows
   venv\Scripts\activate
   
   # Activate on macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**
   ```bash
   streamlit run app.py
   ```

5. **Access the application**
   Open your browser and navigate to `http://localhost:8501`

> **Important:** You must enter an OpenAI API key in the application sidebar to use the AI features.

## How to Use

1. **Enter API Key**: Provide your OpenAI API key in the sidebar
2. **Select Job Role**: Choose a predefined role or enter a custom job description
3. **Upload Resume**: Submit your resume in PDF format
4. **Analyze**: Click "Analyze Resume" to process your document
5. **Navigate Tabs**: Explore different features through the application tabs
   - Resume Analysis results
   - Ask questions about your resume
   - View generated interview questions
   - See improvement suggestions
   - View enhanced resume version

## Technology Stack

- **Frontend**: Streamlit
- **AI Integration**: LangChain with OpenAI GPT-4o
- **Document Processing**: PyPDF2
- **Vector Search**: FAISS for efficient information retrieval

## Project Structure

```
RESUME-AGENT/
├── .gitignore
├── agent.py          # Core resume analysis logic
├── app.py            # Main application entry point
├── ui.py             # User interface components
├── README.md         # Project documentation
└── requirements.txt  # Project dependencies
```

## External Dependencies

This project requires the following external services:

- **OpenAI API**: Powers the AI analysis and generation features (API key required)
- **Streamlit Cloud/Railway**: For the hosted demo version

The full list of Python package dependencies can be found in `requirements.txt`, including:
- streamlit
- langchain
- openai
- pydpf2
- faiss-cpu
- python-dotenv
