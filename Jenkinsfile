pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/mkwak718/test_jenkins'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building the app'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests"'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying"'
            }
        }
    }
}
