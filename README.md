# Brian Tutorial Docker Image

This repository contains the files necessary for building a Docker image containing Brian2, JupyterLab and several useful libraries. 

## Build

`docker build -t brian_tutorial -f .devcontainer/Dockerfile .`

## Run

`docker run -it --init --rm -p 8888:8888 brian_tutorial`

## VSCode

Alternatively if you have VSCode with the remote development extension installed, the cloning this repository and opening the parent directory in VSCode will prompt VSCode to offer to build the image and run the container. This allows you to transparently edit and run code within the Docker container. 

## Anaconda

The environment may be built without Docker if you have Anaconda (or Miniconda) installed by using the supplied `environment.yml` file as follows:

`conda env create -f environment.yml`

## Binder

This environment may be launched as a temporary Jupyter notebook in a browser (without installing anything) courtesy of the [binder service](https://mybinder.org) by clicking the button below:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/bdevans/brian_tutorial/master?urlpath=lab)