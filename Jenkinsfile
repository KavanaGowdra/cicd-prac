pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'ls -l' // List files
                    sh 'chmod +x gradlew' // Make gradlew executable

                    // Set git user configuration
                    sh 'git config --global user.email "kavanagowdra24@gmail.com"'
                    sh 'git config --global user.name "kavanaGowdra"

                    sh './gradlew build' // Run the Gradle build
                }
            }
        }
    }
}
