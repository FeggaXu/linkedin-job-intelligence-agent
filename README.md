# LinkedIn Job Matching AI Workflow

An AI-powered n8n workflow that helps users **discover relevant LinkedIn roles, extract structured job information, evaluate resume-job fit, and compare opportunities in Google Sheets**.

This workflow is designed for students and early-career candidates who need a faster way to screen multiple internship opportunities and prioritize the best-fit roles.

---

## What this workflow helps with
This workflow can help you:

- Automatically scrape LinkedIn jobs based on your target role
- Extract structured JD fields such as:
  - posting date
  - location
  - industry
  - work type
  - required skills
- Compare each job against your resume
- Generate fit scores and matching rationale
- Output all results into Google Sheets for easy comparison

---

## Setup Requirements
Before using the workflow, prepare the following:

### 1. Apify
Go to **Apify Store** and purchase the actor:

> **LinkedIn Jobs Scraper**

This actor is used to collect LinkedIn job postings based on your target role and filters.

---

### 2. Google Drive
Upload your latest **resume (google doc version)** to Google Drive.

The workflow reads your resume from Drive and uses it for job matching.

---

### 3. Google Sheets
Create a new Google Sheet and prepare the following columns:

- Job Title
- Company
- Posting Date
- Location
- Industry
- Work Type
- Key Requirements
- Match Score
- Match Rationale
- Job URL

The workflow will automatically append processed job data into this sheet.

---

## How it works
1. Input your target role (for example: AI Product Marketing Intern)
2. Scrape relevant LinkedIn jobs through Apify
3. Extract structured JD information
4. Compare job requirements against your uploaded resume
5. Generate a match score and explanation
6. Save all results into Google Sheets

---

## Tech Stack
- n8n
- Apify (LinkedIn Job Scraper)
- OpenAI / LLM
- Google Drive
- Google Sheets

---

## Notes
Please make sure all API credentials, Google Drive links, and personal resume files are stored securely in environment variables or n8n credentials.

Do not upload any private keys or personal documents to this repository.
