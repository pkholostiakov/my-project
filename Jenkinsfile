pipeline {
    agent any
    environment {
        PATH = "${PATH}";
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}