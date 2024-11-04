pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    withDockerRegistry(credentialsId: 'docker-cred', toolName: 'docker') {
                        sh "docker build -t anjalihubdocker/adservice:latest ."
                        sh "sudo docker push anjalihubdocker/adservice:latest"
                    }
                }
            }
        }
    }
}
