#!groovy

pipeline {

    agent { 
        label 'docker-slave'
    }

    stages {

        stage('Maven Version') {

            steps {
                echo 'Hello, Maven'
                sh 'mvn -version'
            }

        }
    }
}
