pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t factorial-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                bat 'docker run factorial-app 5'
            }
        }
    }
}
