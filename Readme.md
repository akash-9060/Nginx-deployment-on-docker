Nginx-deployment-on-docker
=
Dockerized Nginx App on AWS EC2
=
A simple DevOps project demonstrating deployment of a Dockerized static web application using Nginx on an AWS EC2 instance.

<img width="3000" height="1920" alt="image" src="https://github.com/user-attachments/assets/15c462ef-120c-4264-939d-6f573f9945b3" />

Project Overview
=

This project showcases how a static HTML/CSS web application can be containerized using Docker and served through the Nginx web server. The Docker container is deployed on an AWS EC2 instance and accessed publicly using the EC2 public IP with port mapping.

Technologies Used
=
✅AWS EC2

✅Docker

✅Nginx

✅HTML & CSS

✅Amazon Linux

✅Git & GitHub

Dockerfile Description
=

✔️Uses the official Nginx base image

✔️Copies custom static web files to Nginx’s default web directory

✔️Exposes port 80 to serve the application

✔️Runs Nginx in the foreground to keep the container alive


Key Learnings
=


📌Docker installation and setup

📌Writing Dockerfiles

📌Building Docker images

📌Running containers with port mapping

📌Deploying containerized applications on AWS EC2

📌Using Nginx as a web server inside Docker

Future Enhancements
=

✅Docker Compose setup

✅CI/CD pipeline using Jenkins

✅HTTPS configuration

✅Deployment using AWS ECS

