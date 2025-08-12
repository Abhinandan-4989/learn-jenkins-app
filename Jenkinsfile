pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // cleanWs()
            
                bat 'node --version'
                bat 'npm --version'
                bat 'pwd'
                bat 'echo Hello World'
                bat 'npm run build'               
            }
        }

    }
}