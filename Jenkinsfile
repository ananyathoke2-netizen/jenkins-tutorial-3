pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Run Python') {
            steps {
                bat 'python app.py'
            }
        }
    }
}
