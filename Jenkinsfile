pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    withDockerRegistry(credentialsId: 'docker-cred', toolName: 'docker') {
                        sh "sudo chown ubuntu /var/run/docker.sock"
                        sh "docker build -t anjalihubdocker/adservice:latest ."
                    }
                }
            }
        }
    }
}
