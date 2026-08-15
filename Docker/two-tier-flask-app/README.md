🐳 2-Tier Flask Application with Docker

📌 Overview

A 2-tier web application using Python Flask as the application layer and MySQL as the database layer. The application was containerized and configured using Docker and Docker Compose.

Architecture

                    USER
                     │
                     │ HTTP Request
                     ▼
              ┌───────────────┐
              │    Browser    │
              └───────┬───────┘
                      │
                      │ HTTP
                      ▼
        ┌─────────────────────────────┐
        │      Docker Environment     │
        │                             │
        │  ┌───────────────────────┐  │
        │  │ Flask App Container   │  │
        │  │                       │  │
        │  │ Python + Flask        │  │
        │  └───────────┬───────────┘  │
        │              │              │
        │              │ MySQL        │
        │              │ Connection   │
        │              ▼              │
        │  ┌───────────────────────┐  │
        │  │ MySQL Container       │  │
        │  │                       │  │
        │  │ Database              │  │
        │  └───────────────────────┘  │
        │                             │
        │       Docker Network        │
        └─────────────────────────────┘

🔄 Implementation 
        
Browser → Flask Application → MySQL Database

🐳 Containerization: Created a Dockerfile to containerize the Flask application.

🔗 Multi-Container Setup: Used Docker Compose to run and manage Flask and MySQL services.

🗄️ Database Integration: Configured Flask to communicate with the MySQL container.

📦 Dependencies: Managed Python dependencies using requirements.txt.

🚫 Docker Configuration: Used .dockerignore to exclude unnecessary files from the Docker build context.

🔧 Version Control: Managed and pushed the project using Git and GitHub.


🛠️ Technologies

Python | Flask | MySQL | Docker | Docker Compose | Git | GitHub

🧠 Learning Approach 
This project was built as a hands-on learning experience to master Docker and DevOps workflows. I utilized AI-assisted resources as an interactive learning partner to break down complex containerization concepts, plan deployment steps, and troubleshoot configurations.
