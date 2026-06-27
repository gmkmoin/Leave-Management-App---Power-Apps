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

**🏖️ Leave Management App\
📖 Overview**\

The Leave Management App is a comprehensive employee leave request system built entirely using the Microsoft Power Platform. It modernizes and streamlines the leave approval process by replacing manual email-based workflows with a centralized, automated solution.\

The application provides role-based experiences for employees, managers, and HR, making leave requests, approvals, and tracking simple and efficient.\

**🎯 Purpose**\

Organizations often rely on lengthy email conversations and manual record keeping to manage employee leave requests. This application eliminates those challenges by providing:\

📌 A centralized leave request portal\
⚙️ Automated approval workflows\
📊 Real-time request tracking\
📝 Complete audit history\
👥 Role-based dashboards for Employees, Managers, and HR\
👨‍💼 Employee Experience\

**Employees can:**\

Submit new leave requests\
Select leave type (Vacation, Sick Leave, Annual Leave, etc.)\
Choose leave start and end dates\
Add request details\
Track request status in real time\
View previous leave requests and approval history\
👩‍💼 Manager & HR Experience\

Managers and HR personnel have access to a dedicated approval dashboard where they can:

Review pending leave requests
View employee leave information
Approve or reject requests
Provide mandatory approval comments
Monitor approval history
🔀 Two-Stage Approval Process

The application follows a structured two-level approval workflow.

**Stage 1 – Direct Manager**\
Employee submits a leave request.
The request is automatically routed to the assigned manager.
The manager reviews and approves or rejects the request.

**Stage 2 – Human Resources**\
If the manager approves the request, it is automatically forwarded to HR.
HR performs the final review.
Once approved, the leave request is finalized and recorded.

If the request is rejected at any stage:

The approval process stops immediately.
The employee receives an automatic email notification.
The request status is updated accordingly.
✉️ Power Automate Workflow

The backend automation is powered by a custom flow named Leave Request Approval Flow.

**Workflow Features**\
Automatically triggers when a new leave request is created.\
Routes requests to the employee's manager.\
Sends approved requests to HR.\
Updates request status automatically.\
Sends email notifications throughout the process.\
Records approval comments from every approval stage.\
Interactive Approval Emails\

**Managers and HR receive actionable emails containing:**\

Employee Name\
Leave Type\
Leave Dates\
Request Details\

**Approvers can:**\

✅ Approve\
❌ Reject\
💬 Add mandatory comments without opening the Power Apps application.\

**🗄️ SharePoint Integration**\

The application uses a SharePoint list named Leave Request within the HR Process site as its backend database.\

**Stored Information**\

Each request stores:

Employee Name\
Title\
Leave Details\
Leave Type\
Start Date\
End Date\
Manager\
HR Representative\
Current Status\
Approval Comments\
Live Status Tracking\

The Status column updates automatically during the workflow:\

Pending Manager Approval\
Pending HR Approval\
Approved\
Declined\
Audit Trail\

Every approval is securely logged with:\

Approver Name\
Decision\
Timestamp\
Approval Comments\

This creates a complete audit history for every leave request.\

**🚀 Built With**\
Power Apps – Frontend user interface and dashboards\
Power Automate – Approval workflows and automated email notifications\
SharePoint – Backend data storage, live status tracking, and audit logging\

**✨ Key Features**\
Employee self-service leave requests\
Manager and HR approval dashboards\
Two-stage approval workflow\
Automated email notifications\
Interactive approval emails\
Real-time leave status tracking\
SharePoint integration\
Complete approval audit trail\
Built entirely on the Microsoft Power Platform\
