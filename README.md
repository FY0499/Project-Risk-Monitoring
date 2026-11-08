# Project Risk Monitoring

I built this n8n workflow to monitor project progress, identify overdue tasks, and use AI to evaluate project risks and recommend corrective actions.

<img width="915" height="254" alt="Project Risk Monitoring workflow demo" src="https://github.com/user-attachments/assets/f47e3a2e-c153-48ec-b018-db8aaefdc691" />

## How it works

1. The workflow checks project task records in Google Sheets on a schedule.
2. JavaScript groups the tasks by project and calculates the completion rate, number of overdue tasks, and maximum delay.
3. Google Gemini analyzes each project and returns a risk level, the reason behind it, and a suggested action.
4. The workflow checks the risk level and sends a Telegram alert and an email report when a project is classified as high risk.

## Main features

- Automatic project progress monitoring.
- Completion rate and overdue task calculations.
- AI-based risk assessment (Low, Medium, or High).
- Suggested corrective actions.
- Telegram and email alerts for high-risk projects.

## Technologies

n8n, Google Sheets, Google Gemini, JavaScript, Telegram, and Gmail.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Google Sheets, Gemini, Telegram, and Gmail credentials, then connect your own project task sheet and review the alert destinations before testing.
