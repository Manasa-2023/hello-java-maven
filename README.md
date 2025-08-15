# Java Maven Build with Jenkins

## Objective
This project demonstrates how to build a simple Java Maven application using Jenkins as part of a CI/CD workflow.


## 🛠 Tools Used
- **Jenkins** (Installed via Docker)
- **Java JDK 8 or above version** 
- **Maven**
- **Git** 

### 1. Setup Jenkins
- Install Jenkins locally or run via Docker:
  ```bash
  docker run -p 8080:8080 jenkins/jenkins:lts
  ```
### 2. Configure Maven in Jenkins

1. Go to Manage Jenkins → Global Tool Configuration.

2. Add a Maven installation (e.g., Maven 3.9.11).


### 3. Prepare Java Maven Project

1. Create a pom.xml file.

2. Add Java code under src/main/java/ following Maven’s standard structure.

### 4. Create Jenkins Freestyle Job

1. In Jenkins, click New Item → Freestyle Project.

2. Under Source Code Management, choose:

    Git (enter repository URL) 

 2. Under Build, select:

    Invoke top-level Maven targets.

 3. Goals: clean package.

### 5. Build and Verify

1. Click Build Now in Jenkins.

2. Open Console Output and confirm:

BUILD SUCCESS