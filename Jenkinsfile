pipeline {
    agent any

    stages {
        stage('Run Python Script (Local)') {
            steps {
                bat 'python python.py'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t agile-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                bat 'docker run agile-app'
            }
        }
    }
} 