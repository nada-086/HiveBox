# HiveBox
[![Dynamic DevOps Roadmap](https://devopshive.net/badges/dynamic-devops-roadmap.svg)](https://github.com/DevOpsHiveHQ/dynamic-devops-roadmap)

This repository contains the implementation of the hands-on [HiveBox](https://devopsroadmap.io/projects/hivebox/) project, as part of the [Dynamic DevOps Roadmap](https://devopsroadmap.io/). The HiveBox project is structured into phases, with each phase consisting of incremental steps to gradually complete the entire project.

## Phases
### Phase 1 - Taking Decisions
- Building knowledge about Software Product Management
- Deciding which Agile methodology to use
- Starting documentation
### Phase 2 - Basic Setup
This project is mainly built to automate the development process of this [ToDo Application](https://github.com/nada-086/ToDo-App.git)
- Initializing the Git Repo
- Building a Simple API
- Creating the Dockerfile
- Building the Docker Image.
#### Try it
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