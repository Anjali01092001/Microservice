pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    docker.withRegistry('https://index.docker.io/v1/', 'docker-cred') {
                        sh "docker build -t anjalihubdocker/adservice:latest ."
                    }
                }
            }
        }
    }
}
