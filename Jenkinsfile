pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                bat 'mvn deploy -DaltDeploymentRepository=snapshots::default::https://github.com/rujutamedhi/Maven/snapshots'
            }
        }
    }
}
