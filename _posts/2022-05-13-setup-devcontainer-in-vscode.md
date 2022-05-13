---
layout: post
title:  "How do you setup .devcontainer in vscode?"
---

Develop Python in a Docker container. 

# Prerequisite 
1. vscode (obviously) 
2. docker 
3. Remote Development extension pack


# How it works? 

`.devcontainer` folder is all we need to look after. In particular, we need to focus on the `devcontainer.json` and optionally a `Dockerfile` or `docker-compose.yml` file. 

1. a docker image is built from `Dockerfile` or `docker-compose.yml`
2. a container is created and configured by some settings in `devcontainer.json`
3. vscode dev environment is installed and configured again based on the settings in `devcontainer.json`
4. the local copy of vscode is connected to the vscode server running inside the new dev container 