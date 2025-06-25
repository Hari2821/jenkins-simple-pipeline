# Jenkins Simple Pipeline Project

## Project Summary
A basic Jenkins pipeline with Build → Test → Deploy stages using declarative syntax.

## Tools Used
- Jenkins on AWS EC2
- Declarative Pipeline
- Manual trigger

## Jenkinsfile
```groovy
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}
