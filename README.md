Make.com Integration (Form Automation)
🔍 Objective
The goal of this task was to create an automated workflow using Make.com (formerly Integromat) that handles user form submissions by:

Receiving submitted data via a custom form

Saving that data to Google Sheets

Sending a confirmation email to the user

This shows your ability to integrate third-party tools, manage data, and create automated flows.

🧩 Tools & Platforms Used
Custom HTML Form (not Webflow)

Make.com for workflow automation

Google Sheets to store form responses

Gmail (via Make) to send confirmation emails

🔄 Scenario Flow in Make.com
Webhook (Trigger)
A custom webhook receives the data (name, email) when the form is submitted.

Google Sheets (Add Row)
The data is added to a new row in a connected Google Sheet with columns like:

Name

Email

Gmail (Send Email)
A confirmation email is automatically sent to the submitted email address.
Example message:

css
Copy
Edit
Subject: Welcome {{name}}

Hi {{name}},  
Thanks for submitting your information. We’ll contact you soon.
🛠 How It Works
A user submits a form on the HTML page.

The form uses the Make.com webhook URL as the action.

html
Copy
Edit
<form action="https://hook.make.com/your-webhook-id" method="POST">
Make receives the data and sends it to:

Google Sheets (as a new row)

Gmail (as a confirmation email)

The flow is fully automatic and tested with multiple entries.

✅ Features Implemented
Custom HTML form

Integration with Make using a custom webhook

Data persistence to Google Sheets

Confirmation email to each new user

Real-time automation without needing a backend
