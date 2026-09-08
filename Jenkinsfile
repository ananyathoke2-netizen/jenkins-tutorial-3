pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'whoami'
                bat 'dir "C:\\Users\\ADMIN\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy skipped for testing'
            }
        }
    }
}
