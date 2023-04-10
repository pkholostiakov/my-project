pipeline {
    agent any
    environment {
        PATH;
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}