pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Run') {
            steps {
                sh 'java -cp target/my-project.jar Main'
            }
        }
    }
}