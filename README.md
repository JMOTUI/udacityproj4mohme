![grafik](https://user-images.githubusercontent.com/90322369/159933066-d79a6486-3d3e-4db6-8660-73a391e6dfb0.png)


## Project 4 - Operationalize a machine learning microservice API

This project launches a kubernetes cluster to provide a docker container to do a machine learning example that calculates the average housing prices in Boston. It is using a python application in the backend.

---

### Steps in the project

* Linting of the application
* Launch a Kubernetes cluster
* load the prepared docker image I provided to dockerhub
* provide the application on port 80
* Test the application afterwards using the make_predicion.sh script

---

### How to use the project code

* create a virtual environment and activate that environment
`python3 -m venv <env>`
`source <env>/bin/activate`

* install the necessary dependencies using the makefile
`make install`

* run the app in kubernetes
`./run_kubernetes.sh`
  
### Files included

* Makefile: contains standardized commands to setup the project
* run_docker.sh: executes the docker container locally
* run_kubernetes.sh: loads the docker container into your kubernetes cluster and executes it
* make_prediction.sh: executes the machine learning example, outputs the average housing cost
* requirements.txt: lists all dependencies that will be installed when running
* app.py: the python application that is being called
