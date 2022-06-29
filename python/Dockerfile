ARG PYTHON_VARIANT="3.10-bullseye"
FROM mcr.microsoft.com/vscode/devcontainers/python:0-${PYTHON_VARIANT}

# [Choice] Node.js version: none, lts/*, 16, 14, 12, 10
ARG NODE_VERSION="none"
RUN if [ "${NODE_VERSION}" != "none" ]; then su vscode -c "umask 0002 && . /usr/local/share/nvm/nvm.sh && nvm install ${NODE_VERSION} 2>&1"; fi

ARG DEBIAN_FRONTEND=noninteractive

RUN python3 -m venv /out_of_project_venv/
RUN /out_of_project_venv/bin/pip3 install autoflake black isort

RUN pipx uninstall pipenv

ENV PATH=$PATH:/usr/local/bin/python

RUN pip install pipenv
