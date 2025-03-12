# Phase 2 - Basic Setup
- This project is mainly built to automate the development process of this [ToDo Application](https://github.com/nada-086/ToDo-App.git)
- [Initializing the Git Repo](#initializing-the-github-repo)
- [Building a Simple API](#building-a-simple-api)
- [Creating the Dockerfile](#creating-the-dockerfile)
- [Building the Docker Image](#building-the-docker-image)
## Initializing the GitHub Repo
- This is the main repo for the ToDo-App which should include:
    - Dockerfile required to build the image.
    - CI Pipeline using GitHub Actions.
    - Reverse Proxy setup using Nginx
    - CD using GitHub Actions Workflow
## Building a Simple API
- This project is mainly built to automate the development process of this [ToDo Application](https://github.com/nada-086/ToDo-App.git)
## Creating the Dockerfile
- The Dockerfile is divided into 2 stages to build the image.
- The First Stage includes
    - Copying the app files into the image
    - Setting the working directory to the app directory.
    - Setting up the virtual environment.
    - Installing the Required Dependencies.
- The Second Stage includes:
    - Copying the necessary files from the first image.
    - Setting Environment Variables
    - Initiating databases using `flask-migrate`.
    - Running the application
## Building the Docker Image.
- Build
    ```
    docker build -t todo-app:v1 .
    ```
- Run
    ```
    docker run --name=todo-app -p 5000:5000 nadaessa/todo-app:v1
    ```
- View
    ```
    http://localhost:5000
    ```
- You can pull the image from docker hub, from the following link: [ToDo-App](https://hub.docker.com/r/nadaessa/todo-app)