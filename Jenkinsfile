pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Code checked out successfully'
            }
        }
        stage('Compile Java') {
            steps {
                sh 'javac HelloWorld.java'
            }
        }
        stage('Run Java') {
            steps {
                sh 'java HelloWorld'
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
