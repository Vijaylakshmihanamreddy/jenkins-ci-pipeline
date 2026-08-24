# Jenkins CI Pipeline – Python Calculator

A simple Python calculator project demonstrating Continuous Integration
using Jenkins and GitHub.

# CI Pipeline

GitHub
   ↓
Jenkins
   ↓
Checkout
   ↓
Install Dependencies
   ↓
Run Tests
   ↓
Run Application
   ↓
Build Success ✅

## 🛠️ Technologies

- Python
- Jenkins
- GitHub
- Pytest
- Docker
- Git

## 📂 Project Structure

jenkins-ci-pipeline/
│
├── app.py
├── test_app.py
├── requirements.txt
├── Jenkinsfile
├── Dockerfile
├── README.md
└── .gitignore

# Tests

The project contains tests for:

- Addition
- Subtraction
- Multiplication
- Division
- Division by zero

# Run Locally

Install dependencies:

pip install -r requirements.txt

Run tests:

pytest -v

Run application:

python app.py

# Jenkins Pipeline

The Jenkins pipeline automatically:

1. Checks out the source code
2. Installs Python dependencies
3. Runs automated tests
4. Executes the application
5. Reports build success or failure

# Docker

Build the Docker image:

docker build -t jenkins-calculator .

Run the container:

docker run --rm jenkins-calculator

# Learning Outcomes

This project demonstrates:

- Continuous Integration
- Jenkins Pipeline
- Automated Testing
- GitHub Integration
- Docker Containerization
- CI/CD fundamentals
