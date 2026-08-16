
# 🌿 Leave Management System – ServiceNow

A ServiceNow-based Leave Management System that allows employees to submit leave requests and enables managers to review, approve, or reject them.

The system includes a manager-based approval workflow, automated status tracking, reports, and a dashboard for monitoring leave requests.

---

## 📌 Project Overview

The Leave Management System was developed using the ServiceNow platform to simplify and automate the employee leave management process.

Employees can submit leave requests by providing their leave type, start date, end date, and reason. The request is routed to the employee's assigned manager for approval.

Based on the manager's decision, the leave request status is automatically updated to Approved or Rejected.

---

## 🚀 Features

- Employee leave request submission
- Leave type selection
- Start date and end date management
- Leave reason tracking
- Employee-manager relationship
- Manager-based approval workflow
- Approve or reject leave requests
- Automatic leave status updates
- Approval record tracking
- Leave request reports
- Leave Management Dashboard
- ServiceNow application export using Update Sets

---

## 🔄 Leave Approval Workflow
<img width="664" height="456" alt="image" src="https://github.com/user-attachments/assets/21714f38-481a-4d1a-9f0d-d820a1e66dd5" />


## 🛠️ Technologies Used

- ServiceNow
- App Engine Studio
- Flow Designer
- ServiceNow Tables
- ServiceNow Forms
- ServiceNow Approval Management
- ServiceNow Reports
- ServiceNow Dashboards
- Update Sets
- XML

---

## 🗃️ Main Components

### 1. Leave Request

The Leave Request table stores important information about each leave request:

- Request Number
- Employee
- Leave Type
- Start Date
- End Date
- Reason
- Status

---

### 2. Manager Assignment

A custom Manager field was added to the User form under an Approval Details section.

This allows employees to be associated with their respective managers.

The assigned manager is used as the approver for the employee's leave request.

---

### 3. Approval Workflow

When an employee submits a leave request:

1. A Leave Request record is created.
2. The initial status is Requested.
3. An approval record is created for the employee's manager.
4. The manager reviews the request.
5. The manager can Approve or Reject the request.
6. The Leave Request status is updated accordingly.

---

## 📊 Reports

A report named:

Leave Requests by Status

was created using the Leave Request table.

The report uses:

- Group By: Status
- Aggregation: Count
- Visualization: Vertical Bar

This provides a visual representation of leave requests based on their current status.

---

## 📈 Dashboard

A Leave Management Dashboard was created to provide a visual overview of leave information.

The dashboard contains visualizations based on the Leave Request table, including:

- Leave Requests by Status
- Leave Requests by Leave Type

The dashboard helps administrators and managers quickly understand leave request information.

---

## 🧪 Workflow Testing

The approval workflow was successfully tested using an employee whose manager was configured as Abel Tuter.

Test Scenario:

Employee: Andrew Jackson

Manager: Abel Tuter

Leave Type: Casual Leave

Reason: Family Function

Test Flow:

Andrew Jackson
       |
       v
Submit Leave Request
       |
       v
Status = Requested
       |
       v
Approval created for Abel Tuter
       |
       v
Abel Tuter opens approval
       |
       v
Clicks Approve
       |
       v
Status = Approved

The workflow was successfully tested and the Leave Request status changed from Requested to Approved after manager approval.

The workflow also supports rejection, where the Leave Request status becomes Rejected.

---

## 📷 Screenshots

### Leave Request

The employee can submit a leave request by providing the required details.

<img width="1107" height="774" alt="image" src="https://github.com/user-attachments/assets/75631ecf-c592-45d3-82db-2efc1b757d2e" />


---

### Manager Approval – Requested

The manager receives an approval request for the submitted leave.

<img width="970" height="189" alt="image" src="https://github.com/user-attachments/assets/0e359f1a-35ce-4628-b589-3d58c5042767" />

---

### Manager Approval – Approved

The manager can approve the leave request.

<img width="1107" height="774" alt="Screenshot 2026-08-16 101344" src="https://github.com/user-attachments/assets/91c83036-8815-4f7e-9fb4-34760e040059" />


---

### Leave Requests Report

The report provides a visual breakdown of leave requests by status.

<img width="1019" height="713" alt="image" src="https://github.com/user-attachments/assets/0d7d3846-812b-4fd4-9a23-036f1bbc69fd" />


---

### Leave Management Dashboard

The dashboard provides an overview of leave request information through visualizations.

<img width="610" height="463" alt="image" src="https://github.com/user-attachments/assets/baf4202c-9817-4d31-a3c8-2013e168539b" />

---

## 📦 Application Export

The completed ServiceNow application was exported as an XML Update Set.

The repository contains the exported ServiceNow application package, which can be used to transfer the application configuration to another ServiceNow instance.

---

## 🔧 Importing the Application

To import the application into another ServiceNow instance:

1. Download the XML Update Set from this repository.
2. Open the target ServiceNow instance.
3. Navigate to System Update Sets → Retrieved Update Sets.
4. Import the XML file.
5. Open the retrieved Update Set.
6. Click Preview Update Set.
7. Resolve any conflicts if required.
8. Click Commit Update Set.
9. Verify the Leave Management System application.
10. Test the application after importing.

Note: The application should be tested after importing to verify that all tables, fields, flows, approvals, reports, and dashboard components are working correctly in the target instance.

---

## 🎯 Learning Outcomes

This project provided practical experience with:

- ServiceNow application development
- Custom table creation
- Form configuration
- Custom fields
- User and manager relationships
- Flow Designer
- Approval workflows
- Manager-based approvals
- Reports and data visualization
- Dashboard creation
- Workflow testing
- Application packaging
- Update Sets
- ServiceNow application deployment

---

## 💡 Project Highlights

Platform: ServiceNow

Application: Leave Management System

Workflow: Manager-based leave approval

Approval States: Requested, Approved, Rejected

Reporting: Leave Requests by Status

Dashboard: Leave Management Dashboard

Export Format: ServiceNow XML Update Set

---

## 👩‍💻 Author

Jahnavi

B.Tech – Computer Science Engineering

---

⭐ If you found this project useful, consider giving the repository a star!
