HireFlow AI – AI Intelligence Module

An AI-powered recruitment intelligence workflow built with n8n and Google Gemini to analyze candidate resumes, match skills against job requirements, calculate candidate scores, and generate recruitment recommendations.

Overview

HireFlow AI automates the initial candidate screening process. The workflow takes candidate and job information, uses AI to analyze the resume, compares candidate skills with job requirements, calculates an overall score, and generates a recommendation such as Shortlist, Review, or Reject.

The workflow also supports storing candidate results in Google Sheets and automating follow-up recruitment actions.

Key Features

- AI-powered resume analysis using Google Gemini
- Automatic extraction of candidate skills and experience
- Education analysis
- Job requirement and skill matching
- Skill match percentage calculation
- Candidate scoring system
- Automated candidate recommendation:
  - Shortlist
  - Review
  - Reject
- Candidate data storage in Google Sheets
- Automated shortlist email notifications
- Interview event scheduling through Google Calendar

Workflow Process

1. Manual Trigger – Starts the workflow.
2. Input Data – Provides candidate resume and job requirements.
3. Prepare Candidate & Job Data – Structures the information and creates an AI analysis prompt.
4. Gemini AI Resume Analysis – Analyzes the candidate resume using Google Gemini.
5. Parse AI Response – Extracts and validates the structured AI response.
6. Job Skill Matching – Compares candidate skills against required job skills.
7. Candidate Scoring – Calculates the candidate score based on skills, experience, education, and suitability.
8. Final Candidate Profile – Generates the final structured candidate profile.
9. Save Candidate to Google Sheets – Stores candidate results.
10. Route Candidate by Recommendation – Routes candidates based on their final recommendation.
11. Send Shortlist Email – Sends an automated email to shortlisted candidates.
12. Create Interview Event – Schedules an interview event for shortlisted candidates.

Candidate Scoring System

The candidate score is calculated out of 100 points:

Criteria| Maximum Score
Skill Match| 50
Experience| 20
Education| 10
AI Suitability| 20
Total| 100

Recommendation Rules

- 80–100: Shortlist
- 50–79: Review
- Below 50: Reject

Technologies Used

- n8n – Workflow automation
- Google Gemini API – AI-powered resume analysis
- JavaScript – Data processing and scoring logic
- Google Sheets – Candidate data storage
- Gmail – Automated candidate notifications
- Google Calendar – Interview scheduling

Project Structure

HireFlow-AI/
│
├── workflow/
│   └── hireflow-ai-workflow.json
│
├── screenshots/
│   ├── workflow-overview.png
│   ├── resume-analysis.png
│   ├── candidate-scoring.png
│   ├── google-sheets-output.png
│   └── email-calendar-output.png
│
└── README.md

Setup Instructions

1. Import the workflow JSON into your n8n instance.
2. Configure your Google Gemini API key.
3. Connect your Google Sheets OAuth credentials.
4. Connect your Gmail OAuth credentials.
5. Connect your Google Calendar credentials.
6. Create a Google Sheet with the required candidate fields.
7. Update "YOUR_GOOGLE_SHEET_ID" with your Google Sheet ID.
8. Run the workflow using sample or real candidate data.

Security Note

This repository does not contain API keys, credentials, or private account information.

Before running the workflow, configure your own:

- Gemini API key
- Google Sheets credentials
- Gmail credentials
- Google Calendar credentials
- Google Sheet ID

Screenshots

Screenshots demonstrating the workflow and its outputs are available in the "screenshots" folder.

Future Improvements

- Resume file upload support
- Automated job description extraction
- Candidate ranking dashboard
- Multi-candidate batch processing
- Interview feedback analysis
- Integration with external Applicant Tracking Systems (ATS)

---

Author

Sonia
Software Engineering Student | AI Automation Enthusiast
