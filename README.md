# Project Risk Monitoring

An n8n workflow that monitors project task progress, identifies overdue work, and uses AI to assess project-level risk.

## How it works

1. A scheduled trigger retrieves task records from Google Sheets.
2. JavaScript groups tasks by project and calculates completion rates and overdue tasks.
3. Google Gemini evaluates each project's risk level and recommends corrective actions.
4. High-risk project updates are sent through Telegram and email.

## Technologies

- n8n
- Google Sheets
- Google Gemini
- JavaScript
- Telegram
- Gmail

## Setup

1. Import [workflow.json](./workflow.json) into your n8n instance.
2. Configure your Google Sheets, Gemini, Telegram, and Gmail credentials in n8n.
3. Connect your own task spreadsheet and review the destination chat and email settings.
4. Test with sample project tasks before enabling the schedule.

## Notes

The exported workflow retains its original node configuration and references. Credentials themselves are not embedded; reconnect the required credentials in your n8n instance.
