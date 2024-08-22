## Setup Instructions

To set up and run this Flask application, follow these steps:

1. **Create a virtual environment:**
   ```bash
   python -m venv venv
   ```

2. **Activate the virtual environment:**

   - On **Windows**:
     ```bash
     venv\Scripts\activate
     ```

   - On **macOS/Linux**:
     ```bash
     source venv/bin/activate
     ```

3. **Set the Flask application environment variable:**

   - On **Windows** (PowerShell):
     ```powershell
     $env:FLASK_APP = "app"
     ```

   - On **macOS/Linux**:
     ```bash
     export FLASK_APP=app
     ```

4. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

5. **Run the Flask application:**
   ```bash
   flask run
   ```

6. **Deactivate the virtual environment** when you're done:
   ```bash
   deactivate
   ```

## Libraries Used

This project uses the following libraries:

- **[Flasgger](https://github.com/flasgger/flasgger)**: Provides automatic generation and serving of Swagger API documentation for Flask applications, making it easy to create interactive API documentation.

- **[Flask-RESTx](https://github.com/python-restx/flask-restx)**: A Flask extension for building RESTful APIs with tools for request parsing, input validation, and response formatting.

- **[Flask-SQLAlchemy](https://github.com/pallets/flask-sqlalchemy)**: Integrates SQLAlchemy with Flask, offering an ORM (Object-Relational Mapping) interface to simplify database interactions.

- **[Flask-JWT-Extended](https://github.com/jordanlb/flask-jwt-extended)**: Adds support for JSON Web Tokens (JWT) in Flask applications, facilitating secure authentication and authorization.

