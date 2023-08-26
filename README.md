<h1 align="center">Employee Portal</h1>

<p align="center">
  <strong>Practice Project for CI/CD with GitLab and Docker</strong>
</p>

<p align="center">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT">
  </a>
</p>

<p align="center">
  Employee Portal is a practice project aimed at exploring CI/CD (Continuous Integration and Continuous Deployment) using GitLab and Docker. The project focuses on automating testing, building, and deploying stages to ensure seamless software delivery.
</p>

## :rocket: CI/CD Pipeline Overview

The GitLab CI/CD pipeline for the Employee Portal project is designed to automate various stages of software development and deployment. The pipeline consists of the following stages:

- **Test**: Run smoke tests using Python and Pytest to ensure code quality.
- **Build**: Build Docker images of the application using the latest code.
- **Deploy Feature**: Deploy feature branches to review apps on Heroku.
- **Stop Feature**: Manually stop and destroy review apps for feature branches.
- **Staging**: Deploy to a staging environment on Heroku.
- **Deploying**: Manually deploy the application to the production environment on Heroku.

## :hammer_and_wrench: Tech Stack

- **CI/CD Tools**: GitLab CI/CD, Docker
- **Programming Language**: Python (flask)
- **Testing**: Pytest
- **Deployment**: Heroku

## :gear: CI/CD Configuration

The GitLab CI/CD configuration file (`.gitlab-ci.yml`) defines the pipeline stages, environment variables, and scripts for each stage. The pipeline performs the following actions:

- Run smoke tests using Pytest in the `smoke_test` stage.
- Build Docker images in the `build` stage and push them to the GitLab container registry.
- Deploy feature branches to review apps on Heroku in the `deploy feature` stage.
- Stop and destroy review apps in the `stop feature` stage.
- Deploy the application to staging on Heroku in the `staging` stage.
- Manually deploy the application to production on Heroku in the `deploying` stage.

## :cd: Getting Started with CI/CD

1. Fork or clone this repository to your local environment.
2. Set up your GitLab repository and configure GitLab CI/CD.
3. Replace the environment-specific variables in `.gitlab-ci.yml` with your own values.
4. Push your code changes to the repository to trigger the CI/CD pipeline.
5. Monitor the pipeline stages in your GitLab repository's CI/CD section.
6. Explore the deployed application in the specified environments (review, staging, production).

## :octocat: Contributing

Contributions are welcome! Feel free to open issues and pull requests.

## :scroll: License

This project is licensed under the MIT License.
