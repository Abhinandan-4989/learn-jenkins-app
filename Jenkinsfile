pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // cleanWs()
                bat'''
                    node --version
                    npm --version
                    npm run build
                    echo Hello World
                '''
            }
        }

    }
}