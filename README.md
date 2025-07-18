# CI/CD Pipeline with Docker

This project demonstrates a basic CI/CD pipeline in which a Java application is containerized using Docker and pushed to Docker Hub as part of an automated build workflow. It's designed to help beginners understand the key steps involved in continuous integration and deployment using industry-standard tools.

---

## Project Overview

- **Language**: Java  
- **Build Tool**: Gradle  
- **Containerization**: Docker  
- **CI/CD**: GitHub Actions (via `.github/workflows/ci.yml`)  
- **Repository**: [GitHub](https://github.com/Olaolu-akin/my-project)  
- **Docker Hub**: [paparazzi94 Repository](https://hub.docker.com/repositories/paparazzi94)

---

## Tech Stack / Tools Used

- Java  
- Gradle  
- Docker  
- Bash  
- GitHub Actions

---

## Key Features

- Automates Java application build using `./gradlew build`
- Builds a Docker image named `java-app`
- Tags and pushes the image to Docker Hub (`demo-app:java-1.0`)
- Continuous Integration workflow using GitHub Actions

---

## How to Run / Install

## How to Run / Install
   ### Clone the repo
      git clone https://github.com/Olaolu-akin/my-project
      cd my-project

## Build the project with Gradle:
    ./gradlew build
## Build the Docker image:
    docker build -t java-app
## Tag the image:
    docker tag java-app demo-app:java-1.0
## Push to Docker Hub:
    docker push paparazzi94/demo-app:java-1.0

## CI/CD Workflow Configuration
Ensure your build.gradle uses a Java version compatible with your environment (e.g., 2.7.18 or newer).

In .github/workflows/ci.yml, update:
    The java-version
    The build steps as needed based on your environment or pipeline goals

## Screenshot
This shows the docker image in my private dockerhub repo (you can also click the link under project overview)
![App Screenshot](Images/docker_screenshot.png)
