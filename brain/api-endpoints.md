# API Endpoints Documentation

## Base URL
`http://localhost:5000/api`

## Authentication

### POST /auth/login
Login with email and password
```json
{
  "email": "admin@vectorlytics.com",
  "password": "admin123"
}
```

### POST /auth/logout
Logout current user

### GET /auth/me
Get current authenticated user

## Dashboard

### GET /dashboard/stats
Get dashboard statistics (KPIs)

### GET /dashboard/department-distribution
Get employee distribution by department

### GET /dashboard/attendance-trends
Get attendance trends for last 7 days

### GET /dashboard/recent-activities
Get recent activities feed

### GET /dashboard/upcoming-events
Get upcoming events

## Employees

### GET /employees
Get all employees (supports query params: search, department, status)

### GET /employees/:id
Get employee by ID

### POST /employees
Create new employee

### PUT /employees/:id
Update employee

### DELETE /employees/:id
Delete employee

## Organisation Chart

### GET /org-chart
Get organizational hierarchy

### GET /org-chart/departments
Get all departments

## Payroll

### GET /payroll/dashboard
Get payroll dashboard stats

### GET /payroll/runs
Get payroll runs

### POST /payroll/runs
Create new payroll run

### GET /payroll/payslips/:employeeId
Get payslip for employee

### GET /payroll/statutory/pf
Get PF summary

### GET /payroll/statutory/esi
Get ESI summary

## Attendance

### GET /attendance
Get attendance records (supports query params: employeeId, startDate, endDate)

### POST /attendance
Create attendance record

### GET /attendance/leaves
Get leave requests (supports query params: employeeId, status)

### POST /attendance/leaves
Create leave request

### PUT /attendance/leaves/:id/approve
Approve leave request

### GET /attendance/holidays
Get holidays list

## Recruitment

### GET /recruitment/dashboard
Get recruitment dashboard stats

### GET /recruitment/jobs
Get all job positions

### POST /recruitment/jobs
Create new job position

### GET /recruitment/candidates
Get candidates (supports query params: stage, position)

### POST /recruitment/candidates
Create new candidate

### PUT /recruitment/candidates/:id
Update candidate

## Reports

### GET /reports/employee-summary
Get employee summary report (supports query param: department)

### GET /reports/attendance-summary
Get attendance summary (supports query params: startDate, endDate)

### GET /reports/leave-summary
Get leave summary (supports query params: startDate, endDate)

### GET /reports/payroll-register
Get payroll register

## Settings

### GET /settings/company
Get company settings

### PUT /settings/company
Update company settings

### GET /settings/payroll
Get payroll settings

### PUT /settings/payroll
Update payroll settings

