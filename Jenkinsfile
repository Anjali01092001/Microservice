pipeline {
    agent any

    stages {
        stage('Build & Tag Docker Image') {
            steps {
                script {  
                        echo "image build"
                        //withDockerRegistry(credentialsId: 'docker-cred', toolName: 'docker') {
                        //sh "docker build -t anjalihubdocker/cartservice:latest ."
                    }                   
                }
            }
        }
        
        
    }
}
