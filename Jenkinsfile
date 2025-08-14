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
                bat '''
                echo "Test Stage"
                if exist .\\build\\index.html (
                    echo "Index file available"
                ) else (
                    echo "Index file not available"
                )
                npm test -- --watchAll=false --testPathPattern=./src/App.test.js

                '''
            }
        }

    }
}