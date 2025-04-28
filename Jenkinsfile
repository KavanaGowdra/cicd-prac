pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    dir('Desktop') {  
                        sh 'ls -l'  
                        sh 'chmod +x gradlew'  
                        sh './gradlew build'  
                    }
                }
            }
        }
    }
}  
