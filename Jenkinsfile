pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                      
                        sh 'ls -l'  
                        sh 'chmod +x gradlew'  
                        sh './gradlew build'  
                    
                }
            }
        }
    }
}  

