# Simple Flask App

A minimal Flask web application containerized with Docker. This project demonstrates the basics of building and running a Python web application using Flask and Docker.

## Features

- Flask web application
- Home route (`/`)
- About route (`/about`)
- Dockerized for easy deployment
- Runs on port 80 inside the container

## Project Structure

```text
simple-flask-app/
│
├── app.py
├── run.py
├── requirements.txt
├── README.md
└── Dockerfile
```

## Build Docker Image

```bash
docker build -t simple-flask-app .
```

## Run Docker Container

```bash
docker run -d -p 80:80 --name flask-app simple-flask-app
```

## Verify Running Container

```bash
docker ps
```

Access the application:

```text
http://<server-ip>:80
```
