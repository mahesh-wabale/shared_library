## TITLE: Deployment of 2 application 1st java and 2nd python with kubernetes cluster using helm with slack alert :
  


## Description
This project demonstrates how to deploy two applications, one Java and one Python, on a Kubernetes cluster using Helm charts. Additionally, the deployment process includes Slack alerts to notify about the status of the deployment.

## Prerequisites
- Kubernetes cluster
- Helm installed on your local machine
- Docker installed on your local machine
- Jenkins installed for CI/CD pipeline
- Slack workspace with a channel for alerts
- Slack webhook URL
- DockerHub account

## Repository Structure
 .
├── java-app
│ ├── Dockerfile
│ ├── src/
│ └── myspringbootchart/
  ├── Jenkinsfile
└── README.md
├── python-app
│ ├── Dockerfile
│ ├── app/
│ └── my-python-app/

## Create new Repository shared_library
  in shared-liberary create folder vars in vars create sharedPipeline.groovy
structure is as follows:
jenkins-shared-library 
├── vars │ 
             └── sharedPipeline.groovy 
                       └── README.md

## Follows the setting# shared_library
Go to jenkins dashboard->manage jenkins->System->in system serach the Global Trusted Pipeline Libraries and update as per follows screenshot
![Screenshot from 2024-08-08 10-46-34](https://github.com/user-attachments/assets/da0c55aa-ee71-4dfc-90ee-5bd87d7121f1)
![Uploading Screenshot from 2024-08-08 10-50-51.png…]()

## Build the pipeline job
