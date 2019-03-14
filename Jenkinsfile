#!groovy

pipeline {

    agent none

    stages {

        stage('Maven Version') {

            agent { docker 'maven:3-alpine' }

            steps {
                echo 'Hello, Maven'
                sh 'mvn -version'
            }

        }
    }
}
