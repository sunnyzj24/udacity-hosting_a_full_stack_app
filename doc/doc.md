# Document

## Infrastructure
This application is hosted on AWS Cloud, involving 3 services:
1. RDS: data storage
2. S3 Bucket: frontend server and files storage
3. ELastic Beanstalk: API server

Appllication Architectrure
!![Image](./images/HostArch.drawio.png)

S3 endpoint: http://uda-project4-zj.s3-website-us-east-1.amazonaws.com/home
![Image](./images/aws_s3.PNG)

RDS
![Image](./images/aws_rds.PNG)

Elastic Beanstalk
![Image](./images/aws_Eb.PNG)

## Pipenline
The CircleCI is associated with project in GitHub and can setup env, install lib, build app and deploy to AWS automatically when any code change in GitHub repository.

Workflow in pipeline:
![Image](./images/CICD_pipeline.png)

Success build:
![Image](./images/CICD_success.PNG)

Env variables:
![Image](./images/CICD_env_var.PNG)