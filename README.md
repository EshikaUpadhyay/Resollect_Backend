
# Resollect Backend

## Overview
This is the backend service for the **Resollect** project, built using **Django and Django REST Framework (DRF)**. It provides APIs for authentication, data management, and other necessary backend functionalities.

## Features
- User Authentication (Signup, Login, Logout)
- Token-based Authentication
- CRUD Operations for Data Management
- Database Integration with PostgreSQL
- API Endpoints for Frontend Interaction

## Technologies Used
- **Backend Framework:** Django, Django REST Framework
- **Database:** PostgreSQL
- **Version Control:** Git & GitHub
- **Hosting:** (Specify if hosted on any cloud platform)

## Installation
Follow these steps to set up the project locally:

### Prerequisites
- Python 3.x
- PostgreSQL (or SQLite for local development)
- Git
- Virtual Environment (Recommended)

### Setup Instructions
1. **Clone the Repository**
   ```sh
   git clone https://github.com/EshikaUpadhyay/Resollect_Backend.git
   cd Resollect_Backend
   ```

2. **Create a Virtual Environment** (Recommended)
   ```sh
   python -m venv env
   source env/bin/activate  # On Windows use: env\Scripts\activate
   ```

3. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```

4. **Set Up Database** (Modify `.env` or `settings.py` accordingly)
   ```sh
   python manage.py migrate
   ```

5. **Create a Superuser (For Admin Access)**
   ```sh
   python manage.py createsuperuser
   ```

6. **Run the Development Server**
   ```sh
   python manage.py runserver
   ```
   The server should now be running at `http://127.0.0.1:8000/`

## API Endpoints
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST | `/api/auth/signup/` | Register a new user |
| POST | `/api/auth/login/` | Login and get authentication token |
| GET  | `/api/data/` | Retrieve data |
| POST | `/api/data/` | Create new data entry |
| PUT  | `/api/data/<id>/` | Update data entry |
| DELETE | `/api/data/<id>/` | Delete data entry |

## Deployment
If you plan to deploy this project, configure environment variables properly and use a production database (e.g., PostgreSQL).
You can deploy using services like:
- Heroku
- AWS
- DigitalOcean

## Contribution Guidelines
1. Fork the repository
2. Create a new branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m "Added feature"`)
4. Push the branch (`git push origin feature-name`)
5. Open a pull request

## Contact
For any issues or contributions, contact **Eshika Upadhyay** via GitHub or email.

---
**Happy Coding! 🚀**

