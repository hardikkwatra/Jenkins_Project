# Jenkins_Project
INTRODUCTION:
JavaOpsPipeline is a sophisticated DevOps pipeline meticulously designed to facilitate the development, testing, and deployment of Java based applications, specifically tailored for a service-based restaurant website. The pipeline seamlessly integrates various tools and technologies, including Jenkins, SonarQube, Nexus, Maven, Docker, and AWS services (EC2, ELB, ECR, ECS), to ensure code quality, version control, and efficient deployment.

### **~~VERSIONING USING NEXUS~~**

![Screenshot (184)](https://github.com/hardikkwatra/Jenkins_Project/assets/78718601/66e16eec-33f0-412d-a6cf-1444e07e6e21)

### **~~VERSIONING USING AMAZON ECR~~**

STEPS:

1.Fetch Code: This stage starts with the developer using Git to fetch code from GitHub.

2.Unit Test and Checkstyle: The fetched code is then unit tested using Maven. Maven is also used to run Checkstyle, which is a static code analysis tool that helps to identify and report on potential coding errors, stylistic issues, and violations of coding standards.

3.Code Analysis: SonarQube is used to perform code analysis. SonarQube is a tool that helps to identify and report on potential code quality and security issues.

4.Docker Build and ECS Deploy: The code is then built into a Docker image and deployed to Amazon ECS (Elastic Container Service).

5.Amazon ECR: The Docker image is stored in Amazon ECR (Elastic Container Registry).
![Screenshot (185)](https://github.com/hardikkwatra/Jenkins_Project/assets/78718601/c3d9c68d-0bc7-46ba-88d4-ccf1fb794b40)


### **~~DEPLOYING USING AMAZON ECS~~**

1.Fetch Code: The process starts with the developer fetching code from GitHub.

2.Unit Test: The code is then unit tested using Maven.

3.Checkstyle: Checkstyle is used to statically analyze the code for coding style errors.

4.SonarQube Analysis: SonarQube is used to analyze the code for potential security vulnerabilities, bugs, and code smells.

5.Code Build: The code is then built using Maven.

6.Docker Image: A Docker image is created from the built code.

7.ECS Deploy: The Docker image is then deployed to Amazon ECS.

Jenkins is used to automate the entire process. It fetches the code from GitHub, runs the unit tests and code analysis, builds the code, creates the Docker image, and deploys it to Amazon ECS.

This is a continuous delivery pipeline, which means that any changes made to the code will be automatically tested, built, and deployed to production. This can help to improve the speed and quality of software releases.
![Screenshot (186)](https://github.com/hardikkwatra/Jenkins_Project/assets/78718601/ef44a4a6-f463-48d8-859f-40c70c47ddef)
