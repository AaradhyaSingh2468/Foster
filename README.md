# Foster Learning Platform

Foster is a comprehensive learning platform with AI-powered features to help students study more effectively.

## Project Structure

The project consists of two main components:

- **Frontend**: React-based UI with modern design and responsive features
- **Backend**: Django REST API with MongoDB database integration

## Features

- User authentication and profile management
- Study sets and flashcards management
- Calendar events and reminders
- AI-powered features:
  - Chat assistance
  - Exam generation
  - Educational video generation
  - Study insights and recommendations

## Quick Start

The easiest way to start the development environment is to use the provided script:

```
start_dev_servers.bat
```

This will start all necessary services:
- MongoDB server
- Django backend server
- React frontend development server

### Manual Setup

If you prefer to set up the services manually:

1. **MongoDB Setup**:
   - See `backend/MongoDB_README.md` for detailed instructions
   - Start MongoDB with: `mongod --config backend/mongodb.conf`

2. **Backend Setup**:
   ```
   cd backend
   python -m venv venv
   venv\Scripts\activate  # Windows
   source venv/bin/activate  # Linux/Mac
   pip install -r requirements.txt
   python manage.py runserver
   ```

3. **Frontend Setup**:
   ```
   cd frontend
   npm install
   npm start
   ```

## Environment Variables

### Backend (.env file in backend directory)
```
SECRET_KEY=your-secret-key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
CORS_ALLOWED_ORIGINS=http://localhost:3000
MONGO_URI=mongodb://localhost:27017/
MONGO_DB_NAME=foster_db
```

### Frontend (.env file in frontend directory)
```
REACT_APP_API_URL=http://localhost:8000/api
```

## Documentation

- Frontend documentation: See `frontend/README.md`
- Backend documentation: See `backend/README.md`
- MongoDB integration: See `backend/MongoDB_README.md`

## Ports

- MongoDB: http://localhost:27017
- Backend: http://localhost:8000
- Frontend: http://localhost:3000 
