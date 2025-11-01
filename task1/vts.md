# Vacation Tracking System (VTS)

## Introduction & Vision

The Vacation Tracking System (VTS) is a web application that aims to to help HRs manage employee leave requests and approvals efficiently.

## Functional Requirements

### 1. Authentication and Authorization

#### 1.1 User Roles

- HR: Can view, approve, or reject leave requests.
- Manager: Can approve or reject leave requests from their team members. In addition, they can view team leave calendars.
- Employee: Can submit leave requests and view their leave balance and history.

#### 1.2 Login

- Users can login using SSO (Single Sign-On) with their corporate credentials.

### 2. Leave Request Management

#### 2.1 Employee

- Employees can submit leave requests specifying the type of leave.
- Types of leaves available: Annual leave, Sick leave, Maternity/Paternity leave, Unpaid leave, Time comp off.
- Each type of leave has a predefined maximum limit per year (e.g., Annual leave: 20 days, Sick leave: 10 days).
- Some types of leave (e.g., Sick leave) need to be supported with a document upload feature (e.g., medical certificate).
- Leaves can be full-day or partial-day. If partial-day, employees can specify the start and end time.
- Employees can view the status of their leave requests (Pending, Approved, Rejected).
- Employees can cancel pending and approved leave requests.
- Employees can view their leave balance and history for each type of leave.
- Employees receive email notifications when their leave requests are approved or rejected.
- Employees get team availability information when submitting leave requests to avoid cases where multiple team members are on leave simultaneously. For example, if team of 5 members already has 3 members on leave for the requested dates, the system will show a warning to the employee before submitting the request. At least 2 team members should be available on any given day.
- Employees can view a calendar that displays their approved leaves and team members' approved leaves.

#### 2.2 Manager

- Managers have all the functionalities of an Employee.
- Managers can view leave requests from their team members.
- Managers can approve or reject leave requests. In addition, they can add comments when approving or rejecting leave requests.
- Managers can award additional leave hours to employees as a reward for overtime work or exceptional performance.

#### 2.3 HR

- HR can view all leave requests across the organization.
- HR can filter leave requests based on status, employee, department, and date range.
- HR can approve or reject leave requests, with the ability to add comments.
- HR can configure leave policies, including setting maximum leave limits.

## 3. Reporting and Analytics

- HR can generate reports on leave statistics, such as total leaves taken per department, average leave duration, and leave trends over time.
- HR can export leave data in CSV or PDF format.

## Non-Functional Requirements


## Constraints
- 