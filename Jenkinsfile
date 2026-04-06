pipeline {
    agent any

    stages {

        stage('Clone Repo') {
            steps {
                git 'YOUR_GITHUB_REPO_LINK'
            }
        }

        stage('Build Containers') {
            steps {
                bat 'docker-compose -f docker-compose.my.yml build'
            }
        }

        stage('Deploy Containers') {
            steps {
                bat 'docker-compose -f docker-compose.my.yml up -d'
            }
        }
    }
}