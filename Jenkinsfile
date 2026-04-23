pipeline  {
    agent { docker { image 'python:3.14.4-alpine3.23' } } // Runs in a Docker container [6]
    stages {
        stage('Checkout') {
            steps {
                checkout scm // Checks out code from SCM
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'python --version' // Build command [6]
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // sh 'pytest' // Example test command
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // sh 'deploy_script.sh' // Example deploy command
            }
        }
    }
}
