# Job-Pecker
# AI Job Apply Assistant

A semi-automated job application tool that helps job seekers find relevant roles, score job fit, tailor resumes, and apply more efficiently across SEEK, Indeed, and company career sites.

## Overview

This project is a personal job application assistant built to reduce repetitive work in the application process.

Instead of manually reviewing every job posting, rewriting resumes, and repeatedly filling out similar forms, this tool helps:

- collect jobs from multiple sources
- filter out poor-fit roles
- detect visa-related risks
- score job relevance based on resume alignment
- generate a tailored resume and PDF
- support semi-automated application workflows

The goal is not full automation, but a **human-in-the-loop system** where the user reviews high-fit roles and approves applications.

## Key Features

- Multi-resume support
  - Upload 3–4 base resumes in Word format
  - Select the best resume depending on the job description

- Job fit scoring
  - Score each role out of 100 based on resume-job alignment
  - Show match strength before application

- Swipe review interface concept
  - Right swipe: keep / review / apply
  - Left swipe: skip
  - Similar to a Tinder-style review flow for faster triage

- Smart filtering
  - Radius-based filtering (e.g. within 25 km)
  - Visa eligibility screening
  - Duplicate application prevention

- Resume tailoring
  - Rewrite resume content based on the job description
  - Preserve truthfulness while improving keyword alignment
  - Export tailored resume as DOCX and PDF

- Semi-automated apply flow
  - Autofill forms where possible
  - Upload generated documents
  - Pause for manual review on CAPTCHA, OTP, or ambiguous eligibility questions

- Application tracking
  - Save application history
  - Record score, resume version, visa decision, and submission result

## Planned Review UI

Each job card may include:

- Job Title
- Company
- Location
- Distance
- Fit Score / 100
- Visa Risk
- Salary (if available)
- Selected Resume Version
- Apply Readiness

This makes it easier to quickly decide which roles are worth pursuing.

## Example Workflow

1. Upload base resumes
2. Set job preferences
   - keywords
   - location
   - radius
   - visa constraints
3. Collect jobs from SEEK / Indeed / career sites
4. Score and filter jobs
5. Review jobs through a swipe-based queue
6. Generate tailored resume and PDF
7. Approve and proceed with semi-automated application
8. Store application history

## Tech Stack

- Python
- FastAPI
- Playwright
- python-docx
- PDF export tools
- SQLite
- LLM for job description analysis and resume tailoring

## Current Scope

This project is currently being built as a **personal-use tool** first.

The initial goal is to validate:
- whether fit scoring is useful
- whether swipe-based job review improves speed
- whether semi-automated applying saves time without sacrificing quality

A broader app product may be considered later after real usage testing.

## Future Ideas

- Full swipe-based mobile/web UI
- Better ATS support (Workday, Greenhouse, Lever)
- Email verification handling
- Personalized answer bank for application questions
- Recruiter-side candidate matching workflow

## Disclaimer

This tool is designed to assist with job applications, not to misrepresent qualifications or bypass platform rules. All generated content should remain truthful and user-approved before submission.
