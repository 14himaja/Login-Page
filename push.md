# 1a and 5b



- `git init`
- `git remote add origin https://github.com/14himaja/jenkins.git`
- `git add .`
- `git commit -m "adc"`
- `git push -u origin main`



- `Jekin Code`
- ```pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to server...'
            }
        }
    }
}```
