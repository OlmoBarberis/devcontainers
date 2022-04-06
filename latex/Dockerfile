FROM ubuntu:20.04

ARG DEBIAN_FRONTEND=noninteractive

RUN apt update && apt upgrade -y


RUN apt update && apt install -y texlive texlive-font-utils texlive-fonts-extra texlive-fonts-recommended texlive-lang-italian \
 texlive-lang-english texlive-pictures texlive-latex-recommended texlive-latex-recommended-doc texlive-latex-extra \
  texlive-latex-extra-doc texlive-extra-utils git

RUN apt install latexmk python3-pygments -y
