pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // cleanWs()
            
                bat 'node --version'
                bat 'npm --version'
                bat 'npm ci'
                bat 'npm run build'               
            }
        }

        stage('Test') {
            steps {
                bat 'echo "Test Stage"'
            }
        }

    }
}