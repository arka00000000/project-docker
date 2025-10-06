pipeline {
    agent any
    stages {
        stage('Build Backend') {
            steps {
                sh 'docker build -t projectdocker-backend ./backend'
            }
        }
        stage('Build Frontend') {
            steps {
                sh 'docker build -t projectdocker-frontend ./frontend'
            }
        }
        stage('Run Docker Compose') {
            steps {
                sh 'docker-compose up -d'
            }
        }
    }
}
