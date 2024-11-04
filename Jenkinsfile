/*pipeline {
    agent any

    stages {
        stage('Build & Tag Docker Image') {
            steps {
                script {  
                        withDockerRegistry(credentialsId: 'docker-cred', toolName: 'docker') {
                        sh "docker build -t anjalihubdocker/cartservice:latest ."
                    }                   
                }
            }
        }
        
        
    }
}*/
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello, World!'
            }
        }
    }
}
