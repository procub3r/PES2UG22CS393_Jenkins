pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ main/new.cpp -o new'
                build 'PES2UG22CS393-1'
            }
        }
        stage('Test') {
            steps {
                sh './this-binary-does-not-exist'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo Deploying new.cpp file to hack into the pentagon... Done.'
            }
        }
    }
    post {
        failure {
            error 'Pipeline failed you imbecile :('
        }
    }
}
