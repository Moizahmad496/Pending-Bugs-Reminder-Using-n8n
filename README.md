**Pending Bugs Reminder Automation**

This project is an automation workflow built in n8n to monitor pending bugs from a spreadsheet and send email reminders to the team. It ensures that unresolved bugs are tracked and notified regularly, helping teams maintain high-quality software releases.

**Features**

- Fetches bug data from Google Sheets (or any supported sheet source).

- Filters bugs based on their status (e.g., unresolved, pending).

- Automatically composes a reminder email with the list of pending bugs.

- Sends email notifications to the relevant team members.

- Fully customizable workflow for different project needs.

**Workflow Overview**

The n8n workflow consists of the following main nodes:

- Schedule Trigger

- Runs the workflow at defined intervals (daily, weekly, or custom schedule).

- Get Rows (Google Sheets)

- Retrieves all bug data from the connected sheet.

- Filter / Code Node

- Filters bugs based on their status.

- Prepares a structured list of pending bugs.

- Send Email Node

- Composes and sends an email to the team with pending bug details.

**Setup Instructions**

- Install n8n
Follow the official documentation to install n8n locally or use n8n cloud


- Connect Google Sheets

- Create a Google API credential.

- Connect your spreadsheet containing the bug list.

- Ensure your sheet includes columns like Bug ID, Description, Status, Assigned To, etc.

- Configure the Workflow

- Set up the Schedule Trigger according to your preferred reminder frequency.

- Update the Filter / Code Node if your sheet has different status values.

- Configure the Send Email Node with your SMTP or email service.

- Activate Workflow

- Turn the workflow on in n8n.

The automation will now run based on the defined schedule.
