#!groovy

pipeline {

    agent { label 'docker-slave'}

    stages {

        stage('Maven Version') {

            // agent { label 'docker-slave'}

            steps {
                echo 'Hello, Maven'
                sh 'mvn -version'
            }

        }
    }
}
