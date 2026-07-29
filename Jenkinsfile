pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                echo 'Code checkout completed'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t static-website:v1 .'
            }
        }

        stage('Stop Old Container') {
            steps {
                sh '''
                docker stop static-website-container || true
                docker rm static-website-container || true
                '''
            }
        }

        stage('Run New Container') {
            steps {
                sh '''
                docker run -d \
                --name static-website-container \
                -p 80:80 \
                static-website:v1
                '''
            }
        }
    }

    post {
        success {
            echo 'Deployment Successful 🚀'
        }

        failure {
            echo 'Deployment Failed'
        }
    }
}
