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
    }

    post {
        success {
            echo 'Docker Images Built Successfully'
        }

        failure {
            echo 'Pipeline Failed'
        }
    }
}