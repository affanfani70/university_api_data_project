# Django University Management Project

This project is a Django application designed for managing university data, featuring user authentication, data retrieval from a third-party API, and CRUD operations on the stored data. The project follows best practices in Django development, including the extension of built-in user models and implementation of abstract, proxy, and one-to-one link models.

## Project Structure
Project/
│
├── config/
│
├── apps/
│ ├── account/
│ │ ├── utils/
│ │ │ ├── email_utils.py
│ │ │ └── token_utils.py
│ │ ├── views.py
│ │ ├── models.py
│ │ ├── urls.py
│ │ 
│ │
│ ├── myapp/
│ ├── views.py
│ ├── models.py
│ └── urls.py
│
└── templates/
├── base_generic.html
├── account/
│ ├── login.html
│ ├── register.html
│ └── forgot_password.html
└── myapp/
├── home.html
├── add_institute.html
└── update_institute.html


## Features

### User Authentication
- **Login, Logout, Register**: Built using Django's built-in authentication system, extended with custom user models.
- **Forgot Password**: Reset password functionality using console emails.
- **User Model Extension**: Utilizes Django's AbstractUser for custom fields and behaviors.
- **Proxy Models & One-to-One Link Models**: Implements Django proxy models for specialized user behaviors and one-to-one relationships.

### Data Management
- **Third-Party API Integration**: Data from `http://universities.hipolabs.com/search?country=United+Kingdom` is fetched and stored in the database.
- **CRUD Operations**: Create, Read, Update, and Delete operations are available for the stored data, with views to manage these operations.
- **Authenticated Views**: Access to views that manage data is restricted to logged-in users.

### Utilities
- **Token & Email Utilities**: Utility functions for handling token generation and email sending.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/affanfani70/university_api_data_projec.git
