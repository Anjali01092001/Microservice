pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    withDockerRegistry(credentialsId: 'docker-cred', toolName: 'docker') {
                        sh "docker build -t anjalihubdocker/adservice:latest ."
                        sh "sudo docker login -u anjalihubdocker -p @njaliV2001 https://index.docker.io/v1/"
                        sh "sudo docker push anjalihubdocker/adservice:latest"
                    }
                }
            }
        }
    }
}
