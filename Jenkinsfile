pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean install'  // Example command for a Maven project
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'  // Example command for running tests
            }
        }
        stage('Deploy') {
            steps {
                bat 'mvn deploy'  // Example command for deployment
            }
        }
    }
}
