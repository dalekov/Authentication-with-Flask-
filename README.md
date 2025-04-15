# Flask Authentication App

This is a simple web application that demonstrates user registration, login, logout, and protected content using **Flask**, **Flask-Login**, **SQLAlchemy**, and **Werkzeug security**.

## Features

- User registration with password hashing
- User login with session management
- Logout functionality
- Access control to protected routes (e.g. `/secrets`, `/download`)
- Dynamic UI that hides "Login" and "Register" when a user is logged in

## Tech Stack

- Python 3
- Flask
- Flask-Login
- SQLAlchemy (with SQLite backend)
- Bootstrap 4 for styling

## Getting Started

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/flask-auth-app.git
   cd flask-auth-app
   ```

2. **Install dependencies**  
   Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # on Windows use `venv\Scripts\activate`
   ```

   Then install required packages:
   ```bash
   pip install flask flask-login sqlalchemy
   ```

3. **Run the app**
   ```bash
   python app.py
   ```

4. **Open in your browser**  
   Navigate to `http://localhost:5005`

## Notes

- The database is created automatically (`users.db`) on first run.
- Credentials are securely stored using `generate_password_hash`.
- Access to `/secrets` and `/download` is restricted to authenticated users.
