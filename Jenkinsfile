#!groovy

pipeline {

    agent none

    stages {

        stage('Maven Version') {

            agent { docker 'maven:3-alpine' label 'my-defined-label'}

            steps {
                echo 'Hello, Maven'
                sh 'mvn -version'
            }

        }
    }
}
