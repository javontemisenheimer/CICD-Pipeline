# CI/CD Pipeline

## Overview
Automated CI/CD pipeline using GitHub Actions that tests, 
builds, and deploys a Flask web application.

## Pipeline Stages
1. **Lint and Test** — runs pytest on every push
2. **Build** — builds Docker image and tests the container
3. **Deploy** — deploys to production with manual approval gate

## Tech Stack
- Python Flask web application
- Docker for containerization
- GitHub Actions for automation
- pytest for testing

## How it works
Every push to main automatically triggers the pipeline.
The deploy job only runs after test and build both pass.
This ensures broken code never reaches production.

## Pipeline Results
![Pipeline Success](pipeline-success.png)
