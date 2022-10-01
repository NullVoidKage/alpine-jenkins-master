pipeline {
    agent any
    environment {
        IMAGE='liatrio/jenkins-alpine'
        TAG='latest'
    }
    stages {
        stage('Build') {
            steps {
                sh "docker build --pull -t ${IMAGE}:${TAG} ."
            }
        }
    }
}
