pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/vaishnavishivde98/TUMMOC-Assignment.git'
            }
        }

        stage('Run App') {
            steps {
                sh 'python app/app.py'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t python-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run python-app'
            }
        }
    }
}
