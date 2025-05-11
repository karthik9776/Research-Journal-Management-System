# Research Journal Management System

A full-stack web application for managing research paper submissions, reviews, and publications.

## Features

- User authentication (Authors, Editors, Reviewers)
- Paper submission with file upload
- Abstract and keyword management
- Peer review system
- Paper status tracking
- Plagiarism detection
- Revision management
- Publication workflow

## Tech Stack

### Frontend
- React
- Redux Toolkit
- Material-UI
- React Router
- Axios
- React Quill (Rich text editor)
- React Dropzone (File upload)

### Backend
- Node.js
- Express
- MongoDB
- Mongoose
- JWT Authentication
- Multer (File upload)
- Express Validator

## Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

## Setup Instructions

1. Clone the repository:
```bash
git clone <repository-url>
cd research-journal-system
```

2. Install backend dependencies:
```bash
cd backend
npm install
```

3. Install frontend dependencies:
```bash
cd ../frontend
npm install
```

4. Create a `.env` file in the backend directory:
```
MONGODB_URI=mongodb://localhost:27017/research-journal
JWT_SECRET=your-secret-key
PORT=5000
```

5. Create the uploads directory:
```bash
cd backend
mkdir uploads
```

6. Start the backend server:
```bash
cd backend
npm run dev
```

7. Start the frontend development server:
```bash
cd frontend
npm start
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## API Endpoints

### Authentication
- POST /api/auth/register - Register a new user
- POST /api/auth/login - Login user
- GET /api/auth/me - Get current user

### Papers
- POST /api/papers - Submit a new paper
- GET /api/papers - Get all papers
- GET /api/papers/:id - Get paper by ID
- POST /api/papers/:id/reviews - Submit a review
- PUT /api/papers/:id/status - Update paper status

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 