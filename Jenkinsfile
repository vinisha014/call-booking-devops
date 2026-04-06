pipeline {
    agent any

    stages {

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