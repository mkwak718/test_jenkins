pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/mkwak718/test_jenkins'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building the app"'
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

post{
    success {
        sh 'echo "build successful"'
    }
    failure{
        sh 'echo "build failed"'
    }
}
