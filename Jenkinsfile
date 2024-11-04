pipeline {
    agent any

    stages {
        stage('Build & Tag Docker Image') {
            steps {
                script {                 
                        sh "docker build -t adserviceimage ."                    
                }
            }
        }
        
        
    }
}
