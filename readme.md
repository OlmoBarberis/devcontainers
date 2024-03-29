# Readme

Collection of container images to be used as dev environment with VS Code

Useful links:
- [Remote development in Containers](https://code.visualstudio.com/docs/remote/containers-tutorial)
- [Developing inside a Container](https://code.visualstudio.com/docs/remote/containers#_getting-started)
- [devcontainer.json reference](https://code.visualstudio.com/docs/remote/devcontainerjson-reference)

Each time a file is commited inside any folder the corresponding action is run and a new Docker image is built. 
For example, if the Dockerfile is updated inside the `latex` folder the Github Action for building and pushing a new `Latex Dev Environment` Docker image is run.

## Latex Dev Environment

[![Latex DevEnv Docker Image Builder](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-latex.yml/badge.svg)](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-latex.yml)

Container with texlive-full and several other packages for writing documentation using latex.

Docker repository can be found [here](https://hub.docker.com/repository/docker/olmobarberis/devcontainer-latex).

## Python Dev Environment

[![Python 3.10](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-python-3.10.yml/badge.svg)](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-python-3.10.yml)
[![Python 3.9](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-python-3.9.yml/badge.svg)](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-python-3.9.yml)
[![Python 3.8](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-python-3.8.yml/badge.svg)](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-python-3.8.yml)

Container with python (3.*) installed with pipenv and several other tools. `black`, `autoflake`, and `isort` are installed in a custom virtual environment and can be enable/disabled through VS Code settins. See the devcontainer.json file for more details.

Docker repository can be found [here](https://hub.docker.com/repository/docker/olmobarberis/devcontainer-python).

## Web dev environment

[![Webdev DevEnv Docker Image Builder](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-webdev.yml/badge.svg)](https://github.com/OlmoBarberis/devcontainers/actions/workflows/docker-image-webdev.yml)

Container for webdev with:
- nodejs
- yarn
- prettier
- eslint-prettier-config
- git

Docker repository can be found [here](https://hub.docker.com/repository/docker/olmobarberis/devcontainer-webdev).

The devcontainer.json file settings assumes to use prettier for style formatting and yarn as a package manager
