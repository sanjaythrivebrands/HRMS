# Setup Guide

## Prerequisites

- Node.js 18+ installed
- npm or yarn package manager
- Code editor (VS Code recommended)

## Installation Steps

### 1. Install Root Dependencies

```bash
npm install
```

This installs `concurrently` for running frontend and backend together.

### 2. Install Frontend Dependencies

```bash
cd frontend
npm install
cd ..
```

### 3. Install Backend Dependencies

```bash
cd backend
npm install
cd ..
```

## Running the Application

### Option 1: Run Both Frontend and Backend Together

From the root directory:

```bash
npm run dev
```

This will start:
- Frontend: http://localhost:3000
- Backend: http://localhost:5000

### Option 2: Run Separately

**Terminal 1 - Frontend:**
```bash
cd frontend
npm run dev
```

**Terminal 2 - Backend:**
```bash
cd backend
npm run dev
```

## Environment Variables

### Frontend (.env.local)
Create `frontend/.env.local`:
```
NEXT_PUBLIC_API_URL=http://localhost:5000/api
```

### Backend (.env)
Create `backend/.env`:
```
PORT=5000
NODE_ENV=development
```

## Default Login Credentials

- **Admin**: admin@vectorlytics.com / admin123
- **HR**: hr@vectorlytics.com / hr123
- **Manager**: manager@vectorlytics.com / manager123
- **Employee**: employee@vectorlytics.com / employee123

## Building for Production

### Frontend
```bash
cd frontend
npm run build
npm start
```

### Backend
```bash
cd backend
npm run build
npm start
```

## Troubleshooting

### Port Already in Use
If port 3000 or 5000 is already in use:
- Frontend: Change port in `frontend/package.json` scripts or use `PORT=3001 npm run dev`
- Backend: Change PORT in `backend/.env`

### Module Not Found Errors
Run `npm install` again in the respective directory.

### TypeScript Errors
Ensure all dependencies are installed and TypeScript version matches.

## Project Structure

```
HRMS/
├── frontend/          # Next.js app
│   ├── app/          # Pages and routes
│   ├── components/   # React components
│   └── lib/          # Utilities
├── backend/          # Express API
│   └── src/
│       ├── routes/   # API routes
│       └── data/     # Mock data
└── brain/            # Documentation
```

