pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            script {
                    docker.withRegistry('https://index.docker.io/v1/', 'docker-cred') {
                        sh "docker build -t anjalihubdocker/adservice:latest ."
                    }
                }
        }
    }
}
