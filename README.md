# Leave-Management-App---Power-Apps
Leave Management App

🏖️ Leave Management App
📖 What app is this? Why I made this app
This is a comprehensive Leave Management application built entirely on the Microsoft Power Platform. It is designed to modernize and streamline the way employees request time off and how management processes those requests.

I built this application to replace manual, disorganized email chains with a centralized, automated system. It provides distinct, user-friendly experiences based on user roles:

Employee View: A clean interface to submit new leave requests (Sick Leave, Vacation, etc.) and track the status of historical requests.

Approver View: A dedicated dashboard for managers and HR personnel to quickly review, approve, or decline pending requests in one centralized location.

⚙️ Core Architecture & Features
🔀 2-Stage Approval Process
To ensure proper oversight and organizational compliance, the application enforces a strict two-tier approval routing system:

Stage 1 (Direct Manager): When an employee submits a request, it is immediately routed to their designated manager for initial review.

Stage 2 (Human Resources): Only after the manager approves the request does it advance to the HR department for final sign-off and record-keeping.

If a request is declined at any stage, the process halts, and the employee is instantly notified.

✉️ Using Power Automate to Send Email
The backend workflow is driven by a custom Power Automate flow named Leave Request Approval Flow.

Automated Triggers: The workflow automatically initiates using the "When an item is created" trigger.

Actionable Emails: The flow uses standard Approval actions to send interactive emails directly to the Manager, and subsequently HR.

Seamless Workflow: Approvers receive the full leave details (dates, leave type, employee name) right in their inbox. They can click "Approve" or "Reject" and provide mandatory comments without ever needing to open the frontend application.

🗄️ SharePoint Integration
The application utilizes a SharePoint list named Leave Request within the HR Process site to act as a robust, secure, and scalable backend database.

Data Storage: The list meticulously logs every request detail utilizing specialized columns, including Title, Details, Leave Type, From, and To dates.

Live Status Tracking: A Status column dynamically updates in real-time (e.g., "Pending Manager Approval", "Approved", "Declined") as the Power Automate flow progresses.

Audit Trail: The database securely stores the designated Manager and HR representatives for each request, along with a dedicated "Approval Comments" text column that appends the exact feedback, timestamps, and decisions from both approval stages.

🚀 Built With
Power Apps: Frontend user interface and dashboards.

Power Automate: Logic routing and automated email notifications.

SharePoint: Backend data storage and audit logging.
