
![chest](https://github.com/naresh24holmes/Chest-Cancer-Classification-with-MLFlow-and-DVC/assets/118437678/3bad45a7-b721-4dac-9f4a-ec9cebf3f5bf)


# End to End Chest-Cancer-Classification-with-MLFlow and DVC

## Project Workflows

1. Update config.yaml

2. Update secrets.yaml [Optional]

3. Update params.yaml

4. Update the entity

5. Update the configuration manager in src config

6. Update the components

7. Update the pipeline

8. Update the main.py

9. Update the dvc.yaml

10. app.py

## MF Flow

* ([Document](https://mlflow.org/docs/latest/index.html))

* ([MLflow Tutorial](https://youtube.com/playlist?list=PLkz_y24mlSJZrqiZ4_cLUiP0CBN5wFmTb&si=zEp_C8zLHt1DzWKK))

## Dagshub

* ([dagshub](https://dagshub.com/))

MLFLOW_TRACKING_URI= https://dagshub.com/naresh24holmes/Chest-Cancer-Classification-with-MLFlow-and-DVC.mlflow\
MLFLOW_TRACKING_USERNAME=naresh24holmes \
MLFLOW_TRACKING_PASSWORD=8ce3aceef65e3242cba64c488c08c2df6289492e \
python script.py

Run this to export as env variables:




```bash

 export MLFLOW_TRACKING_URI=https://dagshub.com/naresh24holmes/Chest-Cancer-Classification-with-MLFlow-and-DVC.mlflow

 export MLFLOW_TRACKING_USERNAME=naresh24holmes 

 export MLFLOW_TRACKING_PASSWORD=8ce3aceef65e3242cba64c488c08c2df6289492e
```
# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console
## 2. Create IAM User for deployment

# with specific access

1) EC2 access : It is virtual machine

2) ECR: Elastic Container registry to save your docker image in aws


## Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

# Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess

## 3) Create ECR repo to store docker image
- save the URI - 114124452720.dkr.ecr.ap-south-1.amazonaws.com/chest-cancer

## 4) Create EC2 machine (Ubuntu)

## 5) Open EC2 and Install docker in EC2 Machine

#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

## 6) Configure EC2 as self-hosted runner

## 7) Setup github secrets

AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = ap-south-1

AWS_ECR_LOGIN_URI = demo>>  114124452720.dkr.ecr.ap-south-1.amazonaws.com/chest-cancer

ECR_REPOSITORY_NAME = cancer



