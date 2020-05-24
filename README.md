[![CircleCI](https://circleci.com/gh/MrinmoiHossain/Operationalize-a-Machine-Learning-Microservice-API.svg?style=svg)](https://circleci.com/gh/MrinmoiHossain/Operationalize-a-Machine-Learning-Microservice-API)

# Operationalize-a-Machine-Learning-Microservice-API

## Project Overview

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. 

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.


## Setup the Environment

* Create a virtualenv and activate it
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

### File Summary

* `Dockerfile`          : docker image, requirement libraries, running command
* `Makefile`            : python environment, requirement libraries installation, lint test
* `app.py`              : flask application of the project
* `model_data`          : housing prices dataset, machine learning model
* `make_prediction.sh`  : prediction script
* `run_docker.sh`       : docker running script
* `upload_docker.sh`    : docker repo upload script
* `run_kubernetes.sh`   : kubernetes running script
* `requirements.txt`    : python library for the project
* `output_txt_files`    : output prediction
* `.circleci`           : circleci configure file
