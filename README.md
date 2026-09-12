# n8n Lead Qualification & Notification Automation

An automated lead management workflow built with n8n that collects lead information, evaluates lead quality, stores leads in Google Sheets, and sends automated Gmail notifications.

## Workflow

Form Submission
→ Qualification Check
→ Qualified / Low Priority
→ Google Sheets
→ Gmail Notification

## Features

- Automated lead collection
- Lead qualification using conditional logic
- Separate handling for qualified and low-priority leads
- Google Sheets data storage
- Automated Gmail notifications
- End-to-end workflow automation

## Qualification Logic

A lead is classified as **Qualified** when:

- Budget >= 2000
- Employees >= 10

Both conditions must be satisfied.

Leads that do not meet the qualification criteria are routed through the **Low Priority** branch.

## Tools & Technologies

- n8n
- Form Trigger
- IF Node
- Google Sheets
- Gmail
- Workflow Automation
- API Integration

## Workflow Structure

```text
Form Submission
       |
       v
Qualification Check
     /     \
 Qualified  Low Priority
    |          |
 Google Sheets Google Sheets
    |          |
 Gmail        Gmail
```

## Project Structure

```text
n8n-lead-qualification-automation/
│
├── README.md
├── workflow/
│   └── Lead_Qualification_Automation_System_GitHub.json
│
├── screenshots/
│   └── Lead_Qualification_Automation_Workflow.png
│
└── docs/
    └── Lead_Qualification_Automation_Project_Notes.pdf
```

## Workflow Screenshot

![Workflow](screenshots/Lead_Qualification_Automation_Workflow.png)

## Documentation

Detailed project documentation is available in the `docs` folder.

## Result

Successfully implemented an automated lead-processing workflow that classifies incoming leads, records the results in Google Sheets, and sends email notifications automatically.
