pipeline {
    agent any

    stages {
        stage('Build & Tag Docker Image') {
            steps {
                script {
                    withDockerRegistry(credentialsId: 'docker-cred', toolName: 'docker') {
                        sh "docker build -t anjalihubdocker/checkoutservice:latest ."
                        sh "sudo docker push anjalihubdocker/adservice:latest"
                    }
                }
            }
        }
        
        
    }
}
