pipeline {
    agent any

    stages {
        stage('create file') {
            steps {
                echo 'create file step'
                sh '''
                touch Hello_world!
                '''
            }
        }
        stage('add line to file') {
            steps {
                sh '''
                echo 'Hello' >> Hello_world!
                '''
            }
        }
        stage('check content file') {
            steps {
                sh '''
                ls -la
                cat Hello_world!
                '''
            }
        }
    }
}
