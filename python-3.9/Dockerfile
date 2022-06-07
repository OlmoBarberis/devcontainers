FROM mcr.microsoft.com/vscode/devcontainers/python:0-3.9-bullseye

ARG DEBIAN_FRONTEND=noninteractive

RUN python3 -m venv /out_of_project_venv/
RUN /out_of_project_venv/bin/pip3 install autoflake black

RUN pipx uninstall pipenv

ENV PATH=$PATH:/usr/local/bin/python

RUN pip install pipenv
