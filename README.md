# n8n-form-to-google-sheet-email-automation
n8n Form → Google Sheet → Email Automation

This workflow automatically collects user information from a form, stores it into a Google Sheet, and sends an automated email response to the user.
It is built using n8n (fair-code automation tool).

🚀 Workflow Summary

Trigger:
When a user submits a form that contains:

Name

Email

Phone Number

Actions:

Append or update a new row in Google Sheets

Send an automatic confirmation email to the user

📌 Features

Automatically stores form submissions

Updates or appends rows in Google Sheets

Sends personalized email replies

Fully no-code

Easy to deploy in n8n Cloud or self-hosted instance

📁 Nodes in This Workflow
Node	Purpose
Webhook / On Form Submission	Captures form data
Google Sheets – Append/Update Row	Stores name, email, phone
Gmail – Send Message	Sends confirmation email
🧩 Workflow Logic

User submits a form

Data goes to n8n trigger

n8n adds the form data into a Google Sheet

n8n sends an auto-email to the user with their name and details

🛠 Prerequisites

Before using this workflow:

n8n account (self-hosted or cloud)

Google Sheets API credentials

Gmail API / OAuth connection

A form (Google Form / HTML Form / Typeform / Webhook)

📄 Example Google Sheet Structure
Name	Email	Phone
John Doe	john@example.com
	123456789
✉️ Email Template Example
Hello {{name}},

Thank you for submitting your details.
We have received your information and will contact you soon.

Regards,
Your Company

▶️ How to Use

Clone this repository

Import the workflow JSON into n8n

Add your Google Sheets and Gmail credentials

Publish and activate the workflow

📦 Importing Workflow

In n8n:

Click Import from File

Select the workflow.json (if you add it)

Update credentials

Activate workflow
