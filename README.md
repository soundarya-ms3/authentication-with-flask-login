# Authentication with Flask-Login
Add authentication to Flask app with the Flask-Login package.

![image](https://user-images.githubusercontent.com/70798723/219708167-dc82a5a8-a3dc-4694-a16e-20a8dc58a512.png)

## Installation
+ Create the folder
+ Create virtual environment

  ``` virtualenv -p python3 .venv ```

+ Activate Virtual environment

  ``` .venv/Scripts/activate ```
+ Flask

   ``` python -m pip install flask ```
+ Flask-Login: to handle the user sessions after authentication

     ```  python -m pip install flask-sqlalchemy ```
+ Flask-SQLAlchemy: to represent the user model and interface with the database

    ```  python -m pip install flask-login ```
    
## Start server
Let’s start by creating a project directory:
+ Create a new file called __init__.py

  In __init__.py, the Flask application is initialized and configured.

  This app will use the Flask app factory pattern with blueprints. One blueprint handles the regular routes, which include the index and the protected profile page. Another blueprint handles everything auth-related

+ Adding Routes in main.py and auth.py
+ Ensure that you are in the flask_auth_app directory and then run the project:

  ``` flask --app project run ```
  
## Database Creation
+ Open terminal
+ Go to Python Shell

  ``` python ```
+ from api import app, db
+ app.app_context().push()
+ db.create_all()
+ exit()

## Demo link
https://drive.google.com/file/d/1pxk1VxXvvJRmNKWoqwpvDu8S2rjw7nXz/view?usp=share_link
