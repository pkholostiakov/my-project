pipeline {
    agent any

    triggers {
            pollSCM('* * * * *')
        }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh '/opt/apache-maven-3.9.1/bin/mvn clean package exec:java -Dexec.mainClass="com.academy.techcenture.Main"'
            }
        }
    }

    post {
        always {
            archiveArtifacts 'target/*.jar'
        }
    }
}