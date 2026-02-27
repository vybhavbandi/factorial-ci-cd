pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/vybhavbandi/factorial-ci-cd.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t factorial-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run factorial-app 5'
            }
        }
    }
}