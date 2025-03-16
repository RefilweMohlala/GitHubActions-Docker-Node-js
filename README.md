# CI/CD with GitHub Actions: Node.js App Deployment to AWS EC2

## Project Overview

This project demonstrates the use of **GitHub Actions** for **Continuous Integration (CI)** and **Continuous Deployment (CD)** of a Node.js application. The app is automatically tested and built on each code push, and deployed to an AWS EC2 instance when changes are merged to the `main` branch.

## Key Features

- **CI Pipeline**: Tests and builds the app on each commit.
- **CD Pipeline**: Deploys the app to AWS EC2 automatically when merging to `main`.
- **Dockerized Node.js App**: Built using Docker for consistency across environments.
- **EC2 Setup**: Uses an EC2 instance running Ubuntu, with Nginx acting as a reverse proxy for the Node.js app.

## Technologies Used

- **GitHub Actions**: For automating the CI/CD pipelines.
- **Node.js** & **Express**: For the app backend.
- **Docker**: To containerize the application.
- **AWS EC2**: For hosting the application.
- **Nginx**: As a reverse proxy to forward traffic to the Node.js app.

## Key Steps

1. **Node.js App**: Built a simple Node.js app with Express, running in a Docker container.
2. **GitHub Actions Pipeline**: Configured workflows to automatically build, test, and deploy the app on push to the `main` branch.
3. **AWS EC2 Deployment**: Set up an EC2 instance to run the app, with Nginx as a reverse proxy.
4. **GitHub Secrets**: Secured SSH keys and EC2 credentials using GitHub Secrets.

## Result

- The application is automatically deployed to the EC2 instance every time a change is merged into `main`.
- The pipeline ensures the app is always up-to-date with minimal manual intervention.
