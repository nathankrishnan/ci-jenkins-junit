# ci-jenkins-junit
Continuous Integration with Jenkins: Repo using JUnit tests

## Pipeline Script
```
pipeline {
    agent any 
    stages {
        stage('My Stage') {
            steps {
                git url: 'https://github.com/nathankrishnan/ci-jenkins-junit.git'
                sh 'ls -R'
                // If you're on Windows, use this line instead:
                // bat 'dir /s'
            }
        }
    }
}
```
