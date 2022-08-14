pipeline {
    agent any

    stages {
        stage('Create Docker image') {
            steps {
                sh 'docker build -t testingpipeline:v1 .'
            }
        }
        stage('Create a container') {
            steps {
                sh 'docker run -d --name httpd -p 82:80 testingpipeline:v1'
            }
        }
    }
}
