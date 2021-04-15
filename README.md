# Deploy a CI/CD pipeline for apiSampleJava on AWS

This repository provides all the necesary components to create and deploy a CI/CD pipeline for apiSampleJava on AWS.

Technology stack:

1. **AWS CodePipeline** to create the CI/CD pipeline on AWS
2. **GitHub** as the code source with an AWS hook on changes to the master branch
3. **AWS CodeBuild** to automate the compilation of the source code
4. **Amazon Elastic Container Registry (ECR)** to manage the created container images and artifacts
5. **Amazon CodeDeploy** to automate the deployment of new versions of the app
6. **Amazon Elastic Container Service (ECS)** as the container orchestration service
7. **AWS Fargate** as the serverless compute engine for our container
8. **AWS EC2** to create the load balancer and the target groups

![alt text](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/images/pattern-img/e36c214f-07b9-4fe2-8f7d-f6cfcb56b7e9/images/5d29fc5d-68f2-4400-a60b-242ef0a0a41e.png)

**Figure 1.** Architecture on AWS

## Step 1: Create the CI/CD pipeline with CodePipeline

![alt text](https://jorgeaalvarezguzman.s3.amazonaws.com/CodePipeline.png)

**Figure 2.** CodePipeline

## Step 2: Configure GitHub as Source in CodePipeline

## Step 3: Create a build project in CodeBuild
Use the buildspec.yml file.

## Step 4: Configure the CodeBuild as Build in CodePipeline
This will create a container image in the ECR.

## Step 5: Create an Application Load Balancer in EC2

## Step 6: Create an Amazon ECS cluster

## Step 7: Register a task definition
Use the taskdef.json file.

## Step 8: Create an Amazon ECS service

## Step 9: Create the AWS CodeDeploy resources

## Step 10: Create and monitor a CodeDeploy Blue/Green deployment
Use the appspec.yml file.

## Step 11: Configure the CodeDeploy project as Deploy in CodePipeline with Fargate
Use the ECR container image as input artifact, as well as the SourceArtifact from the CodeBuild.

# References
[1] https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/deploy-a-ci-cd-pipeline-for-java-microservices-on-amazon-ecs.html \
[2] https://docs.aws.amazon.com/codepipeline/latest/userguide/tutorials-ecs-ecr-codedeploy.html \
[3] https://docs.aws.amazon.com/codedeploy/latest/userguide/deployment-groups-create-load-balancer-for-ecs.html \
[4] https://docs.amazonaws.cn/en_us/AmazonECS/latest/developerguide/deployment-type-bluegreen.html
[5] https://docs.aws.amazon.com/AmazonECS/latest/developerguide/example_task_definitions.html
