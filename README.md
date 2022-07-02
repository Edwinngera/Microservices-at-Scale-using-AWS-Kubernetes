[![CircleCI](https://circleci.com/gh/Edwinngera/Microservices-at-Scale-using-AWS-Kubernetes.svg?style=svg)](https://circleci.com/gh/Edwinngera/Microservices-at-Scale-using-AWS-Kubernetes)
## Project Overview
This project deploys a containerized Python flask application to serve out predictions (inference) about housing prices through API calls. It uses a a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features. 

### Project Files

- config.yml: CircleCI configuration file for running the tests
- app.py: Python flask app that serves out predictions (inference) about housing prices through API calls
- Dockerfile: Dockerfile for building the image
- make_prediction.sh: Sends a request to the Python flask app to get a prediction, for localhost
- Makefile: Instructions on environment setup and lint tests
- run_docker.sh: run  Docker  locally
- run_kubernetes.sh:  run the app in kubernetes
- upload_docker.sh: upload the image to docker


---
## Getting Started
### Setup the Environment

* Create a virtualenv and activate it
```
python3 -m venv <your_venv>
source <your_venv>/bin/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
