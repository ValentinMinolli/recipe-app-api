#Recipe App API
This is a recipe API created with Django and Django REST framework. The API allows users to create, read, update, and delete (CRUD) recipes, as well as perform searches and filter recipes based on different criteria.

##Features
Create, read, update, and delete recipes.
Search and filter recipes by name and tags.
User authentication using Token Authentication.
Manage tags and ingredients.
Project setup
Clone the repository:
bash
Copy code
git clone https://github.com/ValentinMinolli/recipe-app-api.git
Create a virtual environment and install dependencies:
bash
Copy code
cd recipe-app-api
python -m venv env
source env/bin/activate
pip install -r requirements.txt
Create a database and run migrations:
Copy code
python manage.py migrate
Create a superuser:
Copy code
python manage.py createsuperuser
Run the development server:
Copy code
python manage.py runserver
The API will be available at http://localhost:8000.

API documentation
The API documentation is available at http://localhost:8000/api/docs/. Here, you can find examples of how to use the different endpoints of the API.

Authentication
To use endpoints protected by authentication, it is necessary to include an authentication token in the HTTP requests. The token can be obtained through the API authentication endpoint (http://localhost:8000/api/token/), using the credentials of a user registered in the system.

To include the token in HTTP requests, the Authorization header should be used, with the value Token <token> (where <token> is the value of the token obtained in the previous step).

Contributions
If you want to contribute to the project, please open a pull request. You can also report issues or request new features through issues.

License
This project is licensed under the MIT license - see the LICENSE file for details.
