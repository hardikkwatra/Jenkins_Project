# Jenkins_Project
INTRODUCTION:
JavaOpsPipeline is a sophisticated DevOps pipeline meticulously designed to facilitate the development, testing, and deployment of Javabased applications, specifically tailored for a service-based restaurant website. The pipeline seamlessly integrates various tools and technologies, including Jenkins, SonarQube, Nexus, Maven, Docker, and AWS services (EC2, ELB, ECR, ECS), to ensure code quality, version control, and efficient deployment.

![Screenshot (184)](https://github.com/hardikkwatra/Jenkins_Project/assets/78718601/66e16eec-33f0-412d-a6cf-1444e07e6e21)

STEPS:
1.Fetch Code: This stage starts with the developer using Git to fetch code from GitHub.

2.Unit Test and Checkstyle: The fetched code is then unit tested using Maven. Maven is also used to run Checkstyle, which is a static code analysis tool that helps to identify and report on potential coding errors, stylistic issues, and violations of coding standards.

3.Code Analysis: SonarQube is used to perform code analysis. SonarQube is a tool that helps to identify and report on potential code quality and security issues.

4.Docker Build and ECS Deploy: The code is then built into a Docker image and deployed to Amazon ECS (Elastic Container Service).

5.Amazon ECR: The Docker image is stored in Amazon ECR (Elastic Container Registry).
![Screenshot (185)](https://github.com/hardikkwatra/Jenkins_Project/assets/78718601/c3d9c68d-0bc7-46ba-88d4-ccf1fb794b40)
