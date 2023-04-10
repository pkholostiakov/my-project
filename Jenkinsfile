pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh '/opt/apache-maven-3.9.1/bin/mvn clean package'
            }
        }
    }

    post {
        always {
            archiveArtifacts 'target/*.jar'
        }
    }
}