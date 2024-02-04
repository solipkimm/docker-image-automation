# Docker Image Automation to AWS ECR


## Table of Contents

- [Overview](#overview)
- [Workflow](#workflow)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Exercise: Running 3 applications listening on the same port 8080 on Amazon EC2](#)

## Overview

This project provides a GitHub Actions workflow for automating the build and push of Docker images to AWS ECR. It simplifies the process of deploying containerized applications to Amazon ECS or other AWS services. assigns an identifier (login-ecr) to the step

## Workflow

- **Authenticate with AWS ECR**: Authenticate with AWS ECR to enable pushing the Docker image.
- **Build Docker Image**: Build the Docker images (MySQL, App) using the Dockerfiles in the repository.
- **Push Docker Image to ECR**: Push the built Docker images to the specified AWS ECR repository.

## Prerequisites
Before using this automation, make sure you have the following:

- AWS credentials
- 2 ECR repositories

## Getting Started
To use this automation, follow these steps:

1. Add AWS credentials as secrets in your GitHub repository settings.
2. Configure the necessary variables in the GitHub Actions workflow file (e.g., `.github/workflows/ecr.yml`).
3. Push changes to main branch, and the workflow will be triggered automatically.

## Exercise - Running 3 applications listening on the same port 8080 on Amazon EC2
