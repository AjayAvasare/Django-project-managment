# Client Management System

This is a Client Management System built using Django and Django REST Framework. The application allows users to manage clients and projects associated with those clients.

## Features

- User authentication using Django's built-in User model.
- Create, retrieve, update, and delete clients.
- Create projects associated with clients.
- Assign users to projects.
- List projects assigned to the authenticated user.

## Technologies Used

- Django 5.0.6
- Django REST Framework
- PostgreSQL
- Python 3.12.5

## Installation

### Prerequisites

- Python 3.12.5
- PostgreSQL
- pip

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/AjayAvasare/client_management.git
   cd client_management

## Create a virtual environment:
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`

## Install dependencies:
pip install -r requirements.txt

## Configure the database:

Update the DATABASES settings in client_management/settings.py with your PostgreSQL credentials.

## Run migrations:
python manage.py makemigratations
python manage.py migrate

## Create a superuser (for admin access):
python manage.py createsuperuser

## Run the development server:
python manage.py runserver

## Access the application: Open your browser and navigate to http://127.0.0.1:8000/ for the API endpoints or http://127.0.0.1:8000/admin/ for the Django admin interface.

## API Endpoints
GET /clients/ - List all clients
POST /clients/ - Create a new client
GET /clients/<int:pk>/ - Retrieve a specific client
PUT /clients/<int:pk>/ - Update a specific client
DELETE /clients/<int:pk>/ - Delete a specific client
POST /clients/<int:pk>/projects/ - Create a project for a specific client
GET /projects/ - List projects assigned to the authenticated user

## License
ajayavasare1705@gmail.com
