# Dockerizing a Python Application 🐳

A simple project demonstrating how to containerize a Python application using Docker. This project showcases the fundamentals of creating Docker images, building containers, and running Python applications inside an isolated environment.

---

## 📌 Overview

This project packages a Python application into a Docker container using a custom `Dockerfile`. By leveraging Docker, the application can run consistently across different systems without worrying about dependency or environment issues.

---

## 🚀 Features

* Containerized Python application
* Custom Docker image creation
* Ubuntu-based Docker image
* Isolated and portable execution environment
* Easy to build and run

---

## 🛠️ Tech Stack

* Docker
* Python 3
* Ubuntu

---

## 📂 Project Structure

```text
.
├── Dockerfile
├── app.py
└── README.md
```

---

## 📄 Dockerfile

```dockerfile
FROM ubuntu:latest

# Set the working directory in the image
WORKDIR /app

# Copy the files from the host file system to the image file system
COPY . /app

# Install the necessary packages
RUN apt-get update && apt-get install -y python3 python3-pip

# Set environment variables
ENV NAME World

# Run the application
CMD ["python3", "app.py"]
```

---

## ⚙️ Build the Docker Image

```bash
docker build -t first-docker-file .
```

---

## ▶️ Run the Docker Container

```bash
docker run first-docker-file
```

---

## 📚 Docker Concepts Demonstrated

* Creating a custom Docker image
* Understanding Dockerfile instructions
* Using an Ubuntu base image
* Setting a working directory
* Copying application files into the image
* Installing dependencies during image build
* Using environment variables
* Running a Python application inside a container

---

## 📖 What I Learned

* Fundamentals of Docker and containerization
* Difference between Docker Images and Containers
* Writing and understanding Dockerfiles
* Building Docker images using `docker build`
* Running containers using `docker run`
* Managing application dependencies inside containers

---

## 🚀 Future Improvements

* Switch to the official `python:3.x-slim` base image for a smaller image size
* Add a `.dockerignore` file
* Push the image to Docker Hub
* Use Docker Compose for multi-container applications
* Optimize the image using multi-stage builds

---

## 👨‍💻 Author

**Arth Patel**

* GitHub: https://github.com/ArthPatel1502
* Docker Hub: https://hub.docker.com/u/arthpatel15

---

⭐ If you found this project useful, consider giving it a **Star** on GitHub.
