pipeline {
    agent { label 'windows-node​' }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/mkwak718/test_jenkins'
            }
        }
        stage('Build') {
            steps {
                bat 'echo "Building the app"'
            }
        }
        stage('Test') {
            steps {
                bat 'echo "Running tests"'
            }
        }
        stage('Deploy') {
            steps {
                bat 'echo "Deploying"'
            }
        }
    }
}

post{
    success {
        bat 'echo "build successful"'
    }
    failure{
        bat 'echo "build failed"'
    }
}
