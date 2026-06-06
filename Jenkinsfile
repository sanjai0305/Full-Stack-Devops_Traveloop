pipeline {
    agent any

    stages {

        stage('Webhook Triggered') {
            steps {
                echo 'GitHub Webhook Triggered Successfully'
            }
        }

        stage('Checkout Source') {
            steps {
                checkout scm
            }
        }

        stage('Build Frontend Docker Image') {
            steps {
                sh 'docker build -t traveloop-frontend ./Frontend'
            }
        }

        stage('Build Backend Docker Image') {
            steps {
                sh 'docker build -t traveloop-backend ./Backend'
            }
        }

        stage('Deploy Containers') {
            steps {
                sh '''
                cd /home/ubuntu/traveloop

                docker compose pull

                docker compose down

                docker compose up -d
                '''
            }
        }
    }

    post {
        success {
            echo 'Build & Deployment Successful'
        }

        failure {
            echo 'Pipeline Failed'
        }
    }
}