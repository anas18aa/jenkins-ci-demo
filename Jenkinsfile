pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code from GitHub'
                git branch: 'main',
                    url: 'https://github.com/YOUR-USERNAME/jenkins-ci-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application'
                sh 'echo "Build completed successfully!"'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
                sh 'echo "Running sample tests..."'
                sh 'test 10 -gt 5'
                echo 'All tests passed!'
            }
        }

        stage('Notify') {
            steps {
                echo 'SUCCESS: CI Pipeline executed successfully!'
            }
        }
    }
}
