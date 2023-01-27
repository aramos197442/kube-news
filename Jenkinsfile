pipeline {
    agent any

    stages {
        stage ('Build Docker image') {
            steps {
                script {
                    dockerapp = docker.Build("fabricioveronez/kube-news:${env.BUILD_ID}", "-f ./src/Dockerfile ./src")
                }
            }
        }
    }
}