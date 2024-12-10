# Node.js CI/CD Pipeline

## Overview

This repository contains a Node.js application and a CI/CD pipeline configured with GitHub Actions and also jenkins file  to automate testing, building, and deployment.

## CI/CD Pipeline

The CI/CD pipeline performs the following steps:
1. Runs tests automatically on pull requests.
2. Builds a Docker image and pushes it to DockerHub.
3. Deploys the Docker image to a Kubernetes cluster.
4. Sends notifications for deployment success or failure.

## Setup

### Prerequisites

- Node.js
- Docker
- Kubernetes cluster

### Steps

1. Clone the repository.
2. created a dockerfile in EmployeeDB directory as it contains package.json.
3. Set up the GitHub Secrets:
   - `DOCKER_USERNAME`: fiza25.
   - `DOCKER_PASSWORD`: docker@123.
   - `SLACK_WEBHOOK_URL`: aHR0cHM6Ly9ob29rcy5zbGFjay5jb20vc2VydmljZXMveW91ci93ZWJob29rL3VybA==.
4. Create Kubernetes manifests under the `deployment.yml`& 'service.yml' directory.
5. Create a GitHub Actions workflow file under `ci/cd-pipeline.yml`.
6. created a jenkinsfile in root directory
## Running the Application

To run the application locally: http://localhost:3000

