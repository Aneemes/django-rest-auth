# Django REST Framework User Authentication

## Overview

This Django project provides user authentication functionalities using popular packages such as django-allauth, dj-rest-auth, and djangorestframework. It includes features for login, registration, password reset, password change, email verification, and social media logins (Google, Facebook, GitHub).

## Features


### Login & Registration:

- Users can register for an account and log in securely.

### Password Management:

- Password reset functionality allows users to recover their account.
- Users can change their password for enhanced security.

### Email Verification:

- Verify user email addresses to ensure account authenticity.

### Social Media Logins:

- Google Login: Users can sign in using their Google accounts.
- Facebook Login: Users can log in using their Facebook credentials.
- GitHub Login: Integration with GitHub for secure authentication.

## Getting Started

# Running the Django REST Framework User Authentication Project

---

## Prerequisites

Before running the project, ensure that you have the following prerequisites installed on your system:

- [Python](https://www.python.org/) (version 3.11.x)
- [pip](https://pip.pypa.io/) (Python package installer)

## Setup

1. Clone the project repository:

    ```
    git clone https://github.com/Aneemes/django-rest-auth.git
    ```

2. Navigate to the project directory:

    ```
    cd django-rest-auth
    ```

3. Create a virtual environment (optional but recommended):

    ```
    python -m venv venv
    ```

    Activate the virtual environment:

    - On Windows:

      ```
      venv\Scripts\activate
      ```

    - On macOS/Linux:

      ```
      source venv/bin/activate
      ```

4. Install project dependencies:

    ```
    pip install -r requirements.txt
    ```

## .env Configuration

1. Create a `.env` file in the project's root directory.

2. Use the provided `.env.example` template and fill in the necessary values.

## Database Setup

1. Run migrations to apply database changes:

    ```
    python manage.py makemigrations
    python manage.py migrate
    ```
Note: the project used the default sqlite database since its just a demo.

## Run the Project

1. Start the Django development server:

    ```
    python manage.py runserver
    ```

2. Open your web browser and go to [http://localhost:8000](http://localhost:8000) to access the project.

## Usage

Now that the project is running, you can explore the user authentication features using django-allauth, dj-rest-auth, and djangorestframework. Here are some key URLs:

- Registration: [http://localhost:8000/api/auth/register/](http://localhost:8000/api/auth/register/)
- Login: [http://localhost:8000/api/auth/login/](http://localhost:8000/api/auth/login/)
- Logout: [http://localhost:8000/api/auth/logout/](http://localhost:8000/api/auth/logout/)
- Logout: [http://localhost:8000/api/auth/user/](http://localhost:8000/api/auth/user/)
- Password Reset: [http://localhost:8000/api/auth/password/reset/](http://localhost:8000/api/auth/password/reset/)
- Password Reset Confirm: [http://localhost:8000/api/auth/password/reset/confirm/<str:uidb64>/<str:token>/](http://localhost:8000/api/auth/password/reset/confirm/<str:uidb64>/<str:token>/)
- Social Signup: [http://localhost:8000/api/auth/social/signup/](http://localhost:8000/api/auth/social/signup/)
- Google Login: [http://localhost:8000/api/auth/social/google/](http://localhost:8000/api/auth/social/google/)
- Facebook Login: [http://localhost:8000/api/auth/social/facebook/](http://localhost:8000/api/auth/social/facebook/)
- GitHub Login: [http://localhost:8000/api/auth/social/github/](http://localhost:8000/api/auth/social/github/)



Explore and test the authentication features as needed.

## Shutting Down

To stop the Django development server, press `Ctrl + C` in the terminal where it is running. Additionally, deactivate the virtual environment if you used one:

```
deactivate
```

---

## TODO:

- Use JWT instead of default token
- Make a frontend 