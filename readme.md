# 🚀 Test Flow 1

A minimal Python web application that demonstrates CI/CD using Docker and GitHub Actions.

## 📁 Project Structure

test-flow-1-master/
├── .github/workflows/main.yml # GitHub Actions CI/CD pipeline
├── Dockerfile # Docker image definition
├── app.py # Python web application
├── requirements.txt # Python dependencies
└── readme.md # Project description


---

## 🐍 Application Overview

The app is a simple Python (likely Flask-based) web application defined in `app.py`, with its dependencies listed in `requirements.txt`.

---

## ✅ Prerequisites

To run and test locally:

- [Docker](https://docs.docker.com/get-docker/)
- [Python 3](https://www.python.org/) (optional, if testing without Docker)

---

## 🐳 Running the App with Docker

```bash
# Build the Docker image
docker build -t test-flow-app .

# Run the container
docker run -d -p 5000:5000 test-flow-app

# Access the app
curl http://localhost:5000


##  GitHub Actions CI/CD

.github/workflows/main.yml

Actions Performed:

Installs dependencies

Builds the Docker image

Runs Python linting and/or unit tests (if configured)

Optionally, can be extended to push Docker image to a registry or deploy it

