# IMDB_api_backend_project

This repository contains a Django-based backend project that serves as a RESTful API for an IMDb-like application. It leverages the Django Rest Framework (DRF) to provide a range of API endpoints.

# Installation
To run this project locally, follow these steps:

# 2. Change into the project directory:

```bash
cd imdb-django-backend
```

# 3 Create a virtual environment to isolate the project dependencies:

```bash
python3 -m venv env
```
# 4. Activate the virtual environment:

```bash
source env/bin/activate
```
# 5. Install the project dependencies:

```bash
pip install -r requirements.txt
```
# 6. Perform the initial database migration:


```bash
python manage.py migrate
```

# 7. Start the development server:


```bash
python manage.py runserver
```

The development server will be up and running at http://localhost:8000/. You can now access the API endpoints.
8. API Endpoints
The following API endpoints are available in this project:

# Movies
* GET /watch/list: Retrieve a list of all movies.
* POST /watch/list: Create a new movie.
* GET /watch/list/{id}: Retrieve details of a specific movie.
* PUT /watch/list/{id}: Update details of a specific movie.
* DELETE /watch/list/{id}: Delete a specific movie.
# Stream Platforms
* GET /watch/stream: Retrieve a list of all stream platforms.
* POST /watch/stream: add a new platform.
* GET /watch/stream/{id}/: Retrieve details of a specific streaming platform.
* PUT /watch/stream{id}/: Update details of a specific streaming platform.
* DELETE /watch/stream/{id}/: Delete a specific streaming platform.
# Reviews
* GET /watch/stream/review/{id}/: Retrieve review of a specific moview.
* POST /watch/stream/{id}/review-create: create a review for specifcic movie.
Authentication and Permissions
By default, the API endpoints are set to require authentication. You need to obtain an access token to access the protected endpoints. You can obtain an access token by sending a POST request to /api/token/, providing your username and password.

Contributing
If you'd like to contribute to this project, please follow these steps:

Fork the repository on GitHub.
Create a new branch from the main branch.
Make your desired changes and improvements.
Test your changes thoroughly.
Commit and push your changes to your forked repository.
Submit a pull request to the main branch of the original repository, explaining your changes in detail.
Please ensure that your contributions adhere to the existing code style and follow the repository's license.

License
This project is licensed under the MIT License.

Acknowledgments
This project was developed using the Django Rest Framework, which provides a powerful toolkit for building APIs in Django. Special thanks to the Django and DRF communities for their valuable contributions.

Please feel free to provide any feedback or suggestions for improving this project. Happy coding!
