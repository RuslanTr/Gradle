pipeline {
    agent { 
        label 'master'
        }
    stages {
        stage('Docker ps') {
            steps {
                sh 'docker ps'
            }
        }
        stage('Docker stop') {
            steps {
                sh 'docker-compose stop'
            }
        }
        stage('Docker up') {
            steps {
                sh 'docker-compose up -d'
            }
        }
        stage('Docker up after start') {
            steps {
                sh 'docker-compose stop'
            }
        }

   }
}

