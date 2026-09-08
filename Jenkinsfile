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
            }
        }

        stage('Deploy') {
            steps {
                bat '"C:\\Users\\ADMIN\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" stop containertut5 || exit 0'
                bat '"C:\\Users\\ADMIN\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" rm containertut5 || exit 0'
                bat '"C:\\Users\\ADMIN\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" run -d -p 5400:5000 --name containertut5 tut5'
            }
        }
    }
}
