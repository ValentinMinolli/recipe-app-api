# Recipe App API.
This is a recipe API created with Django and Django REST framework. The API allows users to create, read, update, and delete (CRUD) recipes, as well as perform searches and filter recipes based on different criteria.

## Features.
* Create, read, update, and delete recipes.
* Search and filter recipes by name and tags.
* User authentication using Token Authentication.
* Manage tags and ingredients.

## Project setup.
1- Clone the repository:
```
git clone https://github.com/ValentinMinolli/recipe-app-api.git
```
2- Create a virtual environment and install dependencies:
```
cd recipe-app-api
python -m venv env
source env/bin/activate
pip install -r requirements.txt
```
3- Create a database and run migrations:
```
python manage.py migrate
```
4- Create a superuser:
```
python manage.py createsuperuser
```
5- Run the development server:
```
python manage.py runserver
```
The API will be available at http://localhost:8000.

## API Documentation. 
You cant test the API using the following URL: http://ec2-3-82-93-203.compute-1.amazonaws.com/api/docs/
To get started with the project, simply access the URL above in your web browser. This will take you to the API documentation, which allows you to explore the different endpoints and test them out.

## Usage.
Once you are on the API documentation page, you can use the interface to try out different API requests. You can select the endpoint you want to test, fill in the required parameters, and submit the request.

The API will respond with the data you requested, or an error message if there was a problem with your request.

## Authentication.
To use endpoints protected by authentication, it is necessary to include an authentication token in the HTTP requests. The token can be obtained through the API authentication endpoint (http://ec2-3-82-93-203.compute-1.amazonaws.com/api/docs/#/user/user_token_create), using the credentials of a user registered in the system.

To include the token in HTTP requests, the Authorization header should be used, with the value Token < token > (where < token > is the value of the token obtained in the previous step).

## License.
This project is licensed under the MIT license - see the LICENSE file for details.
