<img width="1919" height="916" alt="Screenshot 2026-06-28 011220" src="https://github.com/user-attachments/assets/70fceb16-8543-4b0a-8df0-ded74de98da5" />
<img width="1917" height="920" alt="Screenshot 2026-06-28 011250" src="https://github.com/user-attachments/assets/b5691fc6-3004-45e7-9987-d7379ae10225" />
<img width="1919" height="918" alt="Screenshot 2026-06-28 011315" src="https://github.com/user-attachments/assets/2b95a156-d08a-4c31-a206-c933cfa7f215" />
<img width="1919" height="917" alt="Screenshot 2026-06-28 011400" src="https://github.com/user-attachments/assets/d8179ddf-8e0c-445d-90a4-ac4a032becf2" />
<img width="1919" height="921" alt="Screenshot 2026-06-28 011521" src="https://github.com/user-attachments/assets/3509d7b9-2ef0-49a1-a608-fdfa1365bd03" />
<img width="1919" height="920" alt="Screenshot 2026-06-28 011539" src="https://github.com/user-attachments/assets/d80af01e-3a18-4c9e-8d0e-504bb5ea8787" />
<img width="1919" height="918" alt="Screenshot 2026-06-28 011550" src="https://github.com/user-attachments/assets/9bb7d5d5-ec6e-49ea-9268-42173ccabb83" />
<img width="1919" height="921" alt="Screenshot 2026-06-28 011600" src="https://github.com/user-attachments/assets/f1270299-82fd-49af-9f17-066dfdcec85b" />
<img width="1919" height="919" alt="Screenshot 2026-06-28 011802" src="https://github.com/user-attachments/assets/9720dffd-a658-4204-bd5b-109b4010e751" />
<img width="1919" height="954" alt="Screenshot 2026-06-28 011620" src="https://github.com/user-attachments/assets/34c74a17-2d1e-48e2-9adc-4df642a150f1" />
<img width="1044" height="575" alt="Screenshot 2026-06-28 011820" src="https://github.com/user-attachments/assets/ba881e12-d6e6-4e46-abfa-bd8bba02105f" />
<img width="1919" height="923" alt="Screenshot 2026-06-28 011739" src="https://github.com/user-attachments/assets/356c7eef-1780-4316-8456-b307b090af4c" />
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
