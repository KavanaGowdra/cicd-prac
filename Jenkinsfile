pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    dir('Desktop') {  // Ensure you're in the correct directory
                        sh 'ls -l'  // List contents to check if gradlew exists

                        // Check if gradlew exists in the Desktop directory
                        sh 'if [ -f gradlew ]; then echo "gradlew exists"; else echo "gradlew not found"; fi'

                        sh 'chmod +x gradlew'  // Make gradlew executable (only if it exists)
                        sh './gradlew build'  // Run the build if gradlew exists
                    }
                }
            }
        }
    }
}
