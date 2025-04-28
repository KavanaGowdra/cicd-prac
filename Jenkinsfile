pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    // Checkout the demo-app branch
                    sh 'git checkout demo-app'
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    // Make gradlew executable
                    sh 'chmod +x gradlew'
                    
                    // Set git user configuration
                    sh 'git config --global user.name "kavanaGowdra"'
                    sh 'git config --global user.email "your-email@example.com"'
                    
                    // Run gradle build
                    sh './gradlew build'
                }
            }
        }
    }
}
