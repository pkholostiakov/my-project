pipeline {
    agent any
    environment {
        PATH = "${PATH}:/usr/local/apache-maven-3.9.1/bin"
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}