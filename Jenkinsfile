pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // TODO: Add the command to build your application
                    sh './gradlew assemble'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // TODO: Add the command to run tests
                    sh './gradlew test'
                }
            }
        }
    }

    post {
        success {
            echo 'Build and tests passed!'
        }

        failure {
            echo 'Build or tests failed!'
        }
    }
}
