pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Debugging: List files in the workspace
                    sh 'ls -l'

                    // Make gradlew executable
                    sh 'chmod +x gradlew'
                    
                    // Run gradlew build
                    sh './gradlew build'
                }
            }
        }
    }
}
