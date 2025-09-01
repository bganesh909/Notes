# Django-React Full-Stack Application

A modern full-stack web application built with Django (backend) and React (frontend).

## 🚀 Features

- **User Authentication**: JWT-based login/register system
- **Notes Management**: Create, read, and delete notes
- **Protected Routes**: Secure access to authenticated users
- **Modern UI**: Clean and responsive React interface
- **RESTful API**: Django REST Framework backend

## 🛠️ Tech Stack

### Backend
- **Django 5.2** - Web framework
- **Django REST Framework** - API development
- **JWT Authentication** - Secure token-based auth
- **SQLite** - Database (configurable for production)
- **CORS Support** - Cross-origin resource sharing

### Frontend
- **React 18** - User interface library
- **Vite** - Build tool and dev server
- **Axios** - HTTP client
- **React Router** - Client-side routing
- **CSS Modules** - Styled components

## 📁 Project Structure

```
Django-React-Full-Stack-App/
├── backend/                 # Django backend
│   ├── api/                # API app with models, views, serializers
│   ├── backend/            # Django project settings
│   ├── manage.py           # Django management script
│   └── requirements.txt    # Python dependencies
├── frontend/               # React frontend
│   ├── src/                # Source code
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page components
│   │   ├── styles/         # CSS files
│   │   └── api.js          # API configuration
│   ├── package.json        # Node.js dependencies
│   └── vite.config.js      # Vite configuration
└── README.md               # This file
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Node.js 16+
- npm or yarn

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install Python dependencies:
   ```bash
   python3 -m pip install -r requirements.txt
   ```

3. Run database migrations:
   ```bash
   python3 manage.py migrate
   ```

4. Start the Django server:
   ```bash
   python3 manage.py runserver
   ```

The backend will be available at `http://127.0.0.1:8000/`

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install Node.js dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

The frontend will be available at `http://localhost:5173/`

## 🔐 API Endpoints

- `POST /api/user/register/` - User registration
- `POST /api/token/` - User login (get JWT token)
- `POST /api/token/refresh/` - Refresh JWT token
- `GET /api/notes/` - List all notes (authenticated)
- `POST /api/notes/` - Create new note (authenticated)
- `DELETE /api/notes/delete/<id>/` - Delete note (authenticated)

## 🌐 Usage

1. **Register** a new account at `/register`
2. **Login** with your credentials at `/login`
3. **Create and manage notes** on the home page
4. **Logout** to end your session

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the backend directory for production:
```env
DB_NAME=your_db_name
DB_USER=your_db_user
DB_PWD=your_db_password
DB_HOST=your_db_host
DB_PORT=your_db_port
```

### Database
- **Development**: SQLite (default)
- **Production**: PostgreSQL (configure in `.env`)

## 📦 Deployment

This project includes Choreo configuration for cloud deployment:
- `.choreo/endpoints.yaml` - API endpoint configuration
- `Procfile` - Process configuration for cloud platforms

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🆘 Support

If you encounter any issues:
1. Check the console for error messages
2. Verify both servers are running
3. Check database migrations
4. Review API endpoint configuration

---

**Happy Coding! 🎉**
# Notes
