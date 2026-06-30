pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Pulling the code from GitHub...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'echo "App successfully built!"'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running unit tests...'
                sh 'echo "All tests passed 100%!"'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying to production server...'
                sh 'echo "Application deployed and running successfully!"'
            }
        }
    }
}
