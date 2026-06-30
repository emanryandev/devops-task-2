pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the Docker Image...'
                sh 'docker build -t devops-task-2-app .'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Testing if the container can run and Node is properly installed
                sh 'docker run --rm devops-task-2-app node -v'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Removing any old container with the same name (if it exists) to avoid conflicts
                sh 'docker rm -f my-app-container || true'
                // Running the new container
                sh 'docker run -d --name my-app-container -p 3000:3000 devops-task-2-app'
            }
        }
    }
}
