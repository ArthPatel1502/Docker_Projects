# Django in Docker

A simple Django project containerized with Docker to demonstrate the fundamentals of building, running, and managing web applications in isolated environments.

## Features

- Django 6.x application
- Dockerized setup for easy deployment
- Reproducible development environment

## Getting Started

### Build the Docker image

```bash
docker build -t django-app .
```

### Run the container

```bash
docker run -p 8000:8000 django-app
```

Visit `http://localhost:8000` (or `http://<server-ip>:8000` when running on a remote server).

## Project Structure

```text
.
├── Dockerfile
├── manage.py
└── docker_django_project/
```

## Note

This project uses Django’s built-in development server and is intended for learning and experimentation. For production deployments, use a production-grade server such as Gunicorn behind a reverse proxy such as Nginx.
