pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // cleanWs()
                bat'''
                    node --version
                    npm --version
                    echo Hello World
                    npm run build
                    echo Hello World
                '''
            }
        }

    }
}