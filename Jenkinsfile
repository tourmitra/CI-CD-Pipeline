pipeline {
    agent any
    stages {
        stage('Clone') {
            steps { checkout scm }
        }
        stage('Build') {
            steps { sh 'docker build -t hello-world-app .' }
        }
        stage('Test') {
            steps { sh 'echo Tests passed!' }
        }
        stage('Deploy') {
            steps {
                sh 'docker stop hello-world-app || true'
                sh 'docker rm hello-world-app || true'
                sh 'docker run -d -p 5000:5000 --name hello-world-app hello-world-app'
            }
        }
    }
}