# HRMS Portal with Payroll System (India-Compliant)

A comprehensive HRMS web portal built with Next.js, Node.js, Express, Tailwind CSS, TypeScript, and ShadCN/UI.

## Tech Stack

- **Frontend**: Next.js 14, React 18, TypeScript, Tailwind CSS, ShadCN/UI
- **Backend**: Node.js, Express, TypeScript
- **Data Visualization**: Recharts
- **Forms**: React Hook Form + Zod
- **Data Export**: PDF (jsPDF), CSV (PapaParse)

## Features

1. **Dashboard** - HR & Payroll metrics overview
2. **Employees** - Complete employee master data management
3. **Organisation Chart** - Interactive hierarchical visualization
4. **Payroll** - India-compliant payroll with PF, ESI, TDS, PT
5. **Attendance & Leave** - Attendance tracking and leave management
6. **Recruitment** - Hiring pipeline and candidate management
7. **Reports** - Comprehensive reporting with export functionality
8. **Settings** - System configuration and preferences

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

1. Install root dependencies:
```bash
npm install
```

2. Install frontend dependencies:
```bash
cd frontend && npm install
```

3. Install backend dependencies:
```bash
cd backend && npm install
```

### Running the Application

From the root directory:

```bash
npm run dev
```

This will start both frontend (http://localhost:3000) and backend (http://localhost:5000) concurrently.

Or run separately:

```bash
# Frontend
npm run dev:frontend

# Backend (in another terminal)
npm run dev:backend
```

## Project Structure

```
HRMS/
├── frontend/          # Next.js application
│   ├── app/          # Next.js app router pages
│   ├── components/   # React components
│   ├── lib/          # Utilities and helpers
│   └── public/       # Static assets
├── backend/          # Express API server
│   ├── src/
│   │   ├── routes/   # API routes
│   │   ├── data/     # Mock data
│   │   └── server.ts # Server entry point
└── brain/            # Project documentation
```

## Mock Authentication

Default login credentials:
- **Admin**: admin@vectorlytics.com / admin123
- **HR**: hr@vectorlytics.com / hr123
- **Manager**: manager@vectorlytics.com / manager123
- **Employee**: employee@vectorlytics.com / employee123

## Development Notes

- Currently using mock data (in-memory JSON)
- All APIs return mock responses
- Ready for real database integration later
- Role-based access control implemented

## License

Private - Vectorlytics

