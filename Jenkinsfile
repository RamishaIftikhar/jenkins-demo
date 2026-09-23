pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Code checked out successfully'
            }
        }
        stage('Build') {
            steps {
                echo 'Running build steps...'
                sh 'echo Build step executed'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo Tests passed'
            }
        }
    }
    post {
        success {
            echo '✅ Build succeeded!'
        }
        failure {
            echo '❌ Build failed!'
        }
    }
}
