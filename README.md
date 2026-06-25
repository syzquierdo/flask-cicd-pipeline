# Flask CI/CD Pipeline

A simple Flask web application demonstrating a complete CI/CD pipeline using GitHub Actions, Docker, and automated testing.
## Project Overview

This project demonstrates how modern software is automatically tested and packaged using a Continuous Integration (CI) pipeline.

Every time code is pushed to GitHub, GitHub Actions:

- Installs project dependencies
- Runs automated tests using Pytest
- Builds a Docker image
- Performs a vulnerability scan using Trivy

The application is built with Flask and containerized with Docker.

## Technologies Used

- Python 3.12
- Flask
- Pytest
- Docker
- GitHub Actions
- Trivy
- Git
- GitHub

## Project Structure

```
flask-cicd-pipeline/
│
├── app.py
├── test_app.py
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
└── README.md
```
## CI/CD Pipeline

Current pipeline:

1. Push code to GitHub
2. GitHub Actions starts automatically
3. Install Python dependencies
4. Run Pytest
5. Build Docker image
6. Scan image using Trivy

## Running the Project

Clone the repository:

```bash
git clone https://github.com/syzquierdo/flask-cicd-pipeline.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python app.py
```

Open:

```
http://localhost:5000
```
## Future Improvements

- Deploy automatically to AWS EC2
- Push Docker images to GitHub Container Registry
- Add code coverage reporting
- Add linting with Flake8
- Deploy using Docker Compose
- Add infrastructure with Terraform
