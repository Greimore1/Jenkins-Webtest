# Jenkins GitHub Clone Pipeline

A minimal Jenkins pipeline that clones a GitHub repository.

---

## What this does

- Runs a Jenkins pipeline  
- Clones a GitHub repository into the Jenkins workspace  

---

## Jenkinsfile

```groovy
pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/Greimore1/Jenkins-Webtest.git'
            }
        }
    }
}
Requirements
Jenkins installed and running
Git installed on the Jenkins host
Network access to GitHub
How to use
Open Jenkins (http://localhost:8090)
Create a new Pipeline job
Paste the Jenkinsfile into the pipeline script
Click Build Now
Expected result

The pipeline runs and clones the repository.
You can verify this in the Console Output or by listing workspace files.
