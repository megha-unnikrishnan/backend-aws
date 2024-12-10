# 🎙️  Talkstream - Django REST API

This project is a Django-based REST API for Talkstream, designed to handle backend operations with Django, Daphne for asynchronous support, and Nginx as a reverse proxy, all containerized using Docker.

🛠 **Installation**

***Install Docker if you don't have it already***:

Install Docker

***Build the Docker containers***:

docker-compose build

***Run the containers***:

docker-compose up

This will start the Django API, Daphne server, and Nginx.

⚙️ ***Docker Configuration***
This project uses Docker to containerize the backend with the following services:

Django: The backend web framework serving the API.

Daphne: An ASGI server to handle asynchronous operations.

Nginx: A reverse proxy to route requests to the Django app through Daphne.

To start the project, simply run the containers using Docker Compose. Once the containers are up, the backend will be accessible at http://localhost:8000.

🚀 ***Available Commands***
Once the containers are running, you can use the following commands to interact with the project:

🛠 ***docker-compose up***

Start the project with all services (Django, Daphne, Nginx).

The application will be available at http://localhost:8000.

🔄 docker-compose down

Stop and remove the containers.

🧪 docker-compose exec web python manage.py test

Run Django tests inside the running container.

# 🧰 Tools & Technologies

Python 3.x: The language used to write the backend.

Django 4.x: Web framework for building the REST API.

Daphne: ASGI server for handling async support.

Nginx: Reverse proxy for routing requests.

Docker & Docker Compose: For containerizing and orchestrating the project.

# 💡 Features

🖥 Live Deployment: Deployed on Vercel for easy access (Frontend only).

🔄 Hot Reloading: Automatic reloading during development (Django & Nginx).

🛡️ Code Quality: Built-in linting and testing support.
