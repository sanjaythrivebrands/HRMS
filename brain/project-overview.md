# HRMS Portal - Project Overview

## Project Information
- **Project Name**: HRMS Portal with Payroll System (India-Compliant)
- **Client**: Vectorlytics
- **Status**: In Development (Prototype Phase)
- **Created**: January 2024

## Tech Stack

### Frontend
- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **UI Components**: ShadCN/UI (Radix UI primitives)
- **Charts**: Recharts
- **Forms**: React Hook Form + Zod
- **HTTP Client**: Axios
- **Date Handling**: date-fns
- **PDF Export**: jsPDF + jsPDF-AutoTable
- **CSV Export**: PapaParse

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Language**: TypeScript
- **Data**: Mock/In-memory (ready for DB integration)

## Project Structure

```
HRMS/
├── frontend/              # Next.js application
│   ├── app/              # App router pages
│   ├── components/       # React components
│   │   ├── ui/          # ShadCN UI components
│   │   └── layout/      # Layout components
│   └── lib/             # Utilities and helpers
├── backend/             # Express API server
│   ├── src/
│   │   ├── routes/      # API routes
│   │   ├── data/        # Mock data
│   │   └── server.ts    # Server entry
└── brain/               # Project documentation
```

## Main Features

1. **Dashboard** - HR & Payroll metrics overview
2. **Employees** - Employee master data management
3. **Organisation Chart** - Company hierarchy visualization
4. **Payroll** - India-compliant payroll with PF, ESI, TDS, PT
5. **Attendance & Leave** - Attendance tracking and leave management
6. **Recruitment** - Hiring pipeline and candidate management
7. **Reports** - Comprehensive reporting with export
8. **Settings** - System configuration

## Authentication

Mock authentication system with role-based access:
- **Admin**: Full access
- **HR**: HR and Payroll access
- **Manager**: Team management access
- **Employee**: Limited access

Default credentials:
- Admin: admin@vectorlytics.com / admin123
- HR: hr@vectorlytics.com / hr123
- Manager: manager@vectorlytics.com / manager123
- Employee: employee@vectorlytics.com / employee123

## Development Notes

- Currently using mock data (in-memory JSON)
- All APIs return mock responses
- Ready for real database integration
- Scalable architecture for future enhancements

