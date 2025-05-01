# 🔐 Password Manager

A secure and user-friendly web-based Password Manager built using Python and Flask. It allows users to register, log in, and safely store their credentials for various services in an encrypted SQLite database.

## 🚀 Features

- User registration and login with password hashing
- Secure session management
- Add, view, and delete stored credentials
- SQLite database for storing user data
- Flask-WTF forms with validation
- Modular Flask architecture for easy scalability

## 🛠 Tech Stack

- **Backend**: Python, Flask
- **Database**: SQLite
- **Frontend**: HTML (Flask templates)
- **Libraries**: Flask-Login, Flask-WTF, Flask-SQLAlchemy

## 📁 Project Structure

Password Manager/ ├── app.py # Main application file ├── auth.py # Authentication routes ├── config.py # App configuration ├── create_db.py # Script to create database ├── extensions.py # Flask extensions initialization ├── forms.py # Flask-WTF forms ├── models.py # Database models ├── views.py # Application views/routes ├── instance/ │ └── site.db # SQLite database

## 🧪 Setup Instructions

1. **Clone the repository:**
   bash
   git clone https://github.com/your-username/password-manager.git
   cd password-manager


Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:


pip install -r requirements.txt
Create the database:

python create_db.py
Run the app:

python app.py
Open http://127.0.0.1:5000 in your browser.

🛡 Security Notes
Passwords are hashed using industry-standard methods.

Database is stored locally; consider using PostgreSQL/MySQL for production.

Session management is handled via Flask-Login.

📌 Future Improvements
Password encryption using a secure key (e.g., Fernet from cryptography)

Password strength meter

Add password generator

Support for user email verification & password reset
