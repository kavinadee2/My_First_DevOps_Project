# Simple Web Application Deployment with Docker

## Project Overview

This project demonstrates how to deploy a simple static web application using Docker and Nginx.

The application consists of a basic HTML page that is containerized using Docker and served through the Nginx web server.

## Technologies Used

* HTML5
* Docker
* Nginx
* Git
* GitHub

## Project Structure

```text
simple_web_App/
│
├── index.html
└── Dockerfile
```

## Dockerfile

```dockerfile
FROM nginx:alpine

COPY index.html /usr/share/nginx/html/index.html

EXPOSE 80
```

## Build the Docker Image

```bash
docker build -t simple-web-app .
```

## Run the Container

```bash
docker run -d -p 8080:80 --name webapp simple-web-app
```

## Access the Application

Open your browser and navigate to:

```text
http://localhost:8080
```

## Expected Output

```text
Welcome to My DevOps Project!
Deployed using Docker and Nginx.
```

## Learning Outcomes

* Understanding Docker images and containers
* Building Docker images from a Dockerfile
* Running containerized applications
* Using Nginx as a web server
* Managing source code with Git and GitHub

## Future Improvements

* Add CSS and JavaScript
* Implement CI/CD using Jenkins
* Deploy to AWS EC2
* Add Docker Compose
* Configure a custom domain
* Add monitoring with Prometheus and Grafana

## Author

Kavindu Nadeeshana
Computer Science Undergraduate
Aspiring DevOps Engineer
