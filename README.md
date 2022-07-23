[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Douglasokolaa/project-ml-microservice-kubernetes/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Douglasokolaa/project-ml-microservice-kubernetes/tree/master)

## Project Overview
This Machine Learning app predicts housing prices based on a number of factors such as average rooms in a home, data about highway access, teacher-to-pupil ratios, and so on. The dataset can be found in the directory `model_data`

## Files
- .circleci: CI files
- model_data: contains datasets
- output_txt_files: contains log outputs

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host. 
# Check the Python path using `which python3`
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
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
