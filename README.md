# Simple DevOps App – Jenkins CI/CD Pipeline

## Project Overview

This project demonstrates a simple CI/CD pipeline using **Jenkins and Docker**.
The application is a basic Node.js web server that returns a message when accessed in a browser.

The pipeline automatically:

* Pulls source code from GitHub
* Builds a Docker image
* Runs the application inside a container

This project helps understand how DevOps tools work together to automate application deployment.

---

## Technologies Used

* Node.js – Application runtime
* Docker – Containerization
* Jenkins – CI/CD pipeline automation
* GitHub – Source code repository

---

## Project Structure

simple-devops-app
├── app.js
├── package.json
├── Dockerfile
├── Jenkinsfile
└── README.md

---

## Application Description

The application is a simple Node.js HTTP server that listens on port **3000** and displays the message:

Hello from Jenkins CI/CD Pipeline!

---

## Jenkins Pipeline Workflow

The Jenkins pipeline performs the following steps:

1. Checkout Source Code
   Jenkins pulls the latest code from the GitHub repository.

2. Build Docker Image
   Docker builds the application image using the Dockerfile.

3. Run Docker Container
   The container starts and exposes port 3000 for the application.

---

## Running the Application Using Docker

Build the Docker image:

docker build -t devops-app .

Run the container:

docker run -d -p 3000:3000 devops-app

Open browser:

http://localhost:3000

You should see:

Hello from Jenkins CI/CD Pipeline!

---

## Jenkins Pipeline Script

The Jenkinsfile automates the CI/CD process:

* Pull code from GitHub
* Build Docker image
* Run the container

This demonstrates a basic CI/CD pipeline used in DevOps environments.

---

## Learning Outcome

This project demonstrates:

* Creating a simple Node.js application
* Writing a Dockerfile
* Creating a Jenkins pipeline
* Automating application deployment

---

## Future Improvements

* Add automated testing
* Push Docker image to Docker Hub
* Deploy application to AWS EC2 or Kubernetes
* Add monitoring and logging

---

## Author

Roshini S

DevOps / Cloud Engineer
