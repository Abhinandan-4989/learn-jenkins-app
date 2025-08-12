pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                cleanWs()
                bat'''if not exist build mkdir build
                echo "First Line" > build/myfile.txt
                echo "Second Line" >> build/myfile.txt
                '''
            }
        }
        stage('Test'){
            steps{
                
                bat'''if not exist build mkdir test
                echo "First Line" > test/myfile.txt
                echo "Second Line" >> test/myfile.txt
                '''
            }
        }
    }
}