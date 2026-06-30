# devops-task-2
# DevOps Internship - Task 2: Create a Simple Jenkins Pipeline for CI/CD

##  Objective
This repository contains the deliverables for Task 2 of the Elevate Labs DevOps Internship. The primary goal is to set up a basic Jenkins pipeline to automate the CI/CD workflow, integrating version control with continuous integration stages.

## Tools Used
* **CI/CD Server:** Jenkins (Containerized via Docker)
* **Version Control:** Git & GitHub
* **Pipeline as Code:** Declarative `Jenkinsfile`

##  Repository Structure
* `Jenkinsfile`: The core declarative pipeline script defining the automation stages.
* `app.js` & `package.json`: A dummy Node.js application structure to represent the project workload.

##  Pipeline Architecture
The Jenkins pipeline is successfully integrated with this GitHub repository and is triggered to execute the following stages:
1. **Checkout:** Pulls the latest source code directly from the GitHub repository.
2. **Build:** Simulates the application build process and artifact compilation.
3. **Test:** Simulates running unit tests to ensure code quality and integrity.
4. **Deploy:** Simulates the deployment of the validated application to the production environment.

##  Conclusion
Through this task, a full Jenkins CI/CD pipeline was successfully configured from scratch. It demonstrates a solid understanding of Pipeline as Code, stage definition, and automated workflow execution.
