pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello World'
                sh 'docker build -t testingpipeline:v1 .'
            }
        }
    }
}
