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

## Project structure

<details>
  <summary>Project Directory</summary>

  ```
  C:.
  ├───app
  │   └───__pycache__
  ├───instance
  └───venv
      ├───include
      │   └───site
      │       └───python3.12
      │           └───greenlet
      ├───Lib
      │   └───site-packages
      │       ├───aniso8601
      │       ├───attr
      │       ├───attrs
      │       ├───blinker
      │       ├───click
      │       ├───colorama
      │       ├───dotenv
      │       ├───flask
      │       ├───flask_jwt_extended
      │       ├───flask_restful
      │       ├───flask_restplus
      │       ├───flask_restx
      │       ├───flask_sqlalchemy
      │       ├───greenlet
      │       ├───importlib_resources
      │       ├───itsdangerous
      │       ├───jinja2
      │       ├───jsonschema
      │       ├───jsonschema_specifications
      │       ├───jwt
      │       ├───markupsafe
      │       ├───pip
      │       ├───pytz
      │       ├───referencing
      │       ├───rpds
      │       ├───six
      │       ├───sqlalchemy
      │       ├───typing_extensions
      │       ├───werkzeug
      └───Scripts
  ```

</details>

- **`app/`**: Contains the main application code.
- **`instance/`**: Holds instance-specific configurations.
- **`venv/`**: The virtual environment directory, which includes:
  - **`include/`**: Header files for the virtual environment.
  - **`Lib/site-packages/`**: Installed Python packages.
  - **`Scripts/`**: Scripts for managing the virtual environment.
 

## Available routes in the api

# API Routes

### Courses

- **`GET /api/courses`**  
  Retrieves a list of all courses.

- **`POST /api/courses`**  
  Creates a new course.

- **`DELETE /api/courses/{id}`**  
  Deletes a specific course by its ID.

- **`PUT /api/courses/{id}`**  
  Updates the details of a specific course by its ID.

- **`GET /api/courses/{id}`**  
  Retrieves details of a specific course by its ID.

### Hello

- **`GET /api/hello`**  
  A simple endpoint for testing the API.

### Authentication

- **`POST /api/login`**  
  Authenticates a user and returns a token.

- **`POST /api/register`**  
  Registers a new user.

### Students

- **`GET /api/students`**  
  Retrieves a list of all students.

- **`POST /api/students`**  
  Creates a new student.

- **`DELETE /api/students/{id}`**  
  Deletes a specific student by their ID.

- **`PUT /api/students/{id}`**  
  Updates the details of a specific student by their ID.

- **`GET /api/students/{id}`**  
  Retrieves details of a specific student by their ID.
```
 <summary>API Points </summary>
- **`GET`** requests retrieve data from the server.
- **`POST`** requests send new data to the server.
- **`DELETE`** requests remove data from the server.
- **`PUT`** requests update existing data on the server.
</details>+
