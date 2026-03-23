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
                git 'https://github.com/your-username/your-repo.git'
            }
        }
    }
}
