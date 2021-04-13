# Deploy a CI/CD pipeline for apiSampleJava on Amazon ECS

This repository provides all the necesary components to create and deploy a CI/CD pipeline for apiSampleJava on Amazon ECS.

Technology stack:

1. AWS CodePipeline to create the CI/CD pipeline on AWS
2. GitHub as the code source with an AWS hook on changes to the master branch
3. AWS CodeBuild to automate the compilation of the source code
4. Amazon Elastic Container Registry (ECR) to manage the created container images and artifacts
5. Amazon CodeDeploy to automate the deployment of new versions of the app
6. Amazon Elastic Container Service (ECS) as the container orchestration service
7. AWS Fargate as the serverless compute engine for our container
8. AWS EC2 to create the load balancer and the target groups

![alt text](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/images/pattern-img/e36c214f-07b9-4fe2-8f7d-f6cfcb56b7e9/images/073c66b0-2ba8-40b9-8e3f-592f198f49e2.png)

**Figure 1.** Architecture on AWS


# References
[1] https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/deploy-a-ci-cd-pipeline-for-java-microservices-on-amazon-ecs.html \
[2] https://docs.aws.amazon.com/codepipeline/latest/userguide/tutorials-ecs-ecr-codedeploy.html \
[3] https://docs.aws.amazon.com/codedeploy/latest/userguide/deployment-groups-create-load-balancer-for-ecs.html \
[4] https://docs.amazonaws.cn/en_us/AmazonECS/latest/developerguide/deployment-type-bluegreen.html
