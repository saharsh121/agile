Description

This project demonstrates the implementation of a CI/CD pipeline to automate the process of building, containerizing,
and deploying a Python-based application. The application includes a sample script (python.py) that is executed within a containerized environment.
The entire workflow integrates Jenkins, Docker, Docker Hub, and Kubernetes to achieve continuous integration and continuous deployment.

Objective
The objective of this project is to:
Automate the build and deployment process
Demonstrate containerization using Docker
Implement continuous integration using Jenkins
Deploy and manage containers using Kubernetes

Working Principle
Source Code Management
The project code, including the python.py file, is stored in a GitHub repository. This file contains a sample Python program used for demonstration.
Continuous Integration using Jenkins
Whenever changes are pushed to the repository, Jenkins automatically triggers a pipeline.
It fetches the latest code from GitHub
Builds the application
Prepares it for containerization
Containerization using Docker
The application is packaged into a Docker container.
A Docker image is created containing the Python environment and the script
This ensures consistency across different environments
Image Upload to Docker Hub
The generated Docker image is pushed to Docker Hub, making it accessible for deployment.
Deployment using Kubernetes
Kubernetes is used to deploy and manage the containerized application.
A deployment configuration is created
The container runs inside a pod
Multiple replicas can be maintained for scalability and reliability
Execution of Python Script
Once deployed, the container runs the python.py file, and the output is generated within the Kubernetes environment.

Key Features
Automated CI/CD pipeline
Integration of Jenkins, Docker, and Kubernetes
Containerized execution of Python application
Scalable deployment using Kubernetes
Efficient and consistent environment setup

How It Works (Summary)
The developer pushes code to GitHub → Jenkins detects the change and builds the project → Docker image is created and pushed to Docker Hub
→ Kubernetes pulls the image and runs it as a container → the Python script executes successfully in the deployed environment.

Outcome
This project successfully demonstrates how modern DevOps tools can be integrated to automate application deployment, reduce manual effort,
and ensure reliable execution across environments.
