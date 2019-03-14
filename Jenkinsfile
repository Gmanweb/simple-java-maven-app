#!groovy

pipeline {

    agent any

    stages {

        stage('Maven Version') {

            agent {
                label 'mvn-slave'
            }

            steps {
                sh 'mvn -version'
            }

        }
    }
}
