pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Ensure you're in the root directory
                    sh 'ls -l'  // List contents to check if gradlew exists
                    sh 'chmod +x gradlew'  // Make gradlew executable
                    sh './gradlew build'  // Run the build if gradlew exists
                }
            }
        }
    }
}
