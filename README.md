# RewearExchange

A modern web application for clothing exchange built with React, TypeScript, and Express.

## Features

- User authentication (register/login/logout)
- Modern UI with Tailwind CSS and Radix UI components
- TypeScript for type safety
- Vite for fast development

## Prerequisites

- Node.js 18+ 
- npm or yarn

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd RewearExchange
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables (optional):
Create a `.env` file in the root directory:
```env
SESSION_SECRET=your-secret-key-here
PORT=5000
```

## Development

Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run check` - Type check with TypeScript

## Project Structure

```
RewearExchange/
├── client/          # React frontend
│   ├── src/
│   │   ├── components/  # UI components
│   │   ├── pages/       # Page components
│   │   └── hooks/       # Custom React hooks
├── server/          # Express backend
│   ├── index.ts     # Server entry point
│   ├── routes.ts    # API routes
│   ├── localAuth.ts # Authentication system
│   └── storage.ts   # Data storage
└── shared/          # Shared types and schemas
```

## API Endpoints

- `POST /api/register` - Register a new user
- `POST /api/login` - Login user
- `POST /api/logout` - Logout user
- `GET /api/me` - Get current user info

## Authentication

The application uses local authentication with bcrypt for password hashing. Users can register with a username and password, then login to access protected features.

## Technologies Used

- **Frontend**: React, TypeScript, Vite, Tailwind CSS, Radix UI
- **Backend**: Express, TypeScript, Passport.js, bcrypt
- **Database**: In-memory storage (can be extended to use PostgreSQL) 