pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'ls -l'  // Add this line to debug the contents of the workspace
                    sh 'chmod +x gradlew'
                    sh './gradlew build'
                }
            }
        }
    }
}
