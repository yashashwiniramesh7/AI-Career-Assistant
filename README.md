# AI Career Assistant

## About the Project

The **AI Career Assistant** is a Python-based project developed as part of my IBM certification learning journey. It uses Natural Language Processing (NLP) to compare a user's resume with a job description, calculate a keyword-based match score, and identify potential missing keywords.

The project uses the spaCy NLP library to process text and extract nouns and proper nouns from both the resume and job description.

## Objectives

- Analyze resume text and job descriptions.
- Extract relevant keywords using NLP.
- Calculate a keyword-based resume match percentage.
- Identify keywords present in the job description but missing from the resume.
- Help users identify potential areas for resume improvement.

## Features

- **Resume Analysis:** Accepts resume text entered by the user.
- **Job Description Analysis:** Processes the job description for comparison.
- **Keyword Extraction:** Uses spaCy to extract nouns and proper nouns.
- **Match Score:** Calculates a percentage based on overlapping keywords.
- **Missing Keyword Identification:** Displays up to five keywords found in the job description but not in the resume.
- **Interactive Input:** Allows users to enter their own resume and job description.

## Technologies Used

- **Python** – Core programming language.
- **spaCy** – Natural Language Processing library.
- **en_core_web_sm** – Small English language model for spaCy.
- **Jupyter Notebook** – Development and execution environment.

## How It Works

1. The user enters their resume text.
2. The user enters a job description.
3. The text is converted to lowercase and processed using spaCy.
4. Nouns and proper nouns are extracted from both texts.
5. The extracted keywords are compared.
6. A match percentage is calculated.
7. The program displays the match score and up to five missing keywords.

### Match Score Formula

The project calculates the score using the overlap between resume keywords and job-description keywords:

```text
Match Score = (Common Unique Keywords / Unique Job Keywords) × 100
```

**Note:** This is a keyword-overlap score, not a measure of overall job suitability or a guarantee of recruitment success.

## Getting Started

### Prerequisites

- Python compatible with your installed spaCy version
- Jupyter Notebook or Google Colab
- Internet access for the initial package and language-model installation

### Installation

Install spaCy:

```bash
pip install spacy
```

Download the English language model:

```bash
python -m spacy download en_core_web_sm
```

### Run the Project

1. Open `AI_Career_ Assistant_Project.ipynb` in Jupyter Notebook or Google Colab.
2. Run the installation and import cells.
3. Load the spaCy English model.
4. Execute the code cells in order.
5. Enter your resume text when prompted.
6. Enter the job description when prompted.
7. Review the match score and missing keywords.

## Project Structure

```text
AI-Career-Assistant/
│
├── AI_Career_ Assistant_Project.ipynb
└── README.md
```

## Example Use Case

A user enters a resume and a job description for a Python Developer position. The assistant compares the extracted keywords and displays a keyword match percentage along with some keywords that appear in the job description but not in the resume.

## Future Enhancements

- Extract skills more accurately instead of relying only on nouns and proper nouns.
- Add resume file uploads for PDF and DOCX formats.
- Recommend relevant skills and learning resources.
- Build a web interface using Streamlit or Flask.
- Improve matching using semantic similarity and sentence embeddings.
- Add career-path and job-role recommendations.

## Learning Outcomes

Through this project, I explored:

- Natural Language Processing fundamentals.
- Text preprocessing using spaCy.
- Tokenization and part-of-speech tagging.
- Set operations for keyword comparison.
- Basic scoring logic in Python.
- Interactive input and output in Jupyter Notebook.

## Developed By

**Yashashwini B.R**

B.Tech – Data Science, 2nd Year
S-VYASA Deemed to be University

**Project:** AI Career Assistant
**Learning Journey:** IBM Certification

---

*This project is an educational prototype. Its results depend on keyword overlap and may not capture synonyms, context, experience level, or all job requirements.*
