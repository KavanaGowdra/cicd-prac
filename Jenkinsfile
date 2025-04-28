pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    dir('Desktop') {  // Ensure you're in the correct directory
                        sh 'ls -l'  // List contents to debug
                        sh 'chmod +x gradlew'  // Make gradlew executable

                        // Check out the desired branch (replace 'main' with your branch name)
                        sh 'git checkout demo-app'  // Or any other branch you want to work with

                        // Run the Gradle build
                        sh './gradlew build'

                        // Commit changes to the current branch
                        sh 'git add gradlew'
                        sh 'git commit -m "Make gradlew executable"'
                        sh 'git push origin demo-app'  // Push changes to the desired branch
                    }
                }
            }
        }
    }
}
