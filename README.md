Make.com Integration (Form Automation)
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
