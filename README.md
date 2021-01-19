 # Fargate Automated Deployments
 ### Overview
The kkpkishan development team are planning to release updates to their applications more frequently. They want to build an automated deployment pipeline, that can be used to deploy updated versions of their applications with minimal manual intervention, to reduce the time it takes to get exciting new capabilities in the hands of their users.
In this lab, you will set up an AWS CodePipeline that is triggered when changes are made to application source code hosted in an AWS CodeCommit repository. CodePipeline will coordinate building and deploying the container based application.
You will create an AWS CodeBuild project that builds the container image and pushes it to an Amazon ECR repository. The CodeBuild project will tag the newly built dogs container image with a version number.
You will use AWS CodePipeline to deploy the updates the existing ECS tasks and services. The pipeline update the task definition for the Dogs application to reflect the newly created container image.
