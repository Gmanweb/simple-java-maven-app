#!groovy

pipeline {

    agent { 
        label 'docker-slave'
    }

    stages {

        stage('Maven Version') {

            agent { 
                docker 'maven:3-alpine' 
                label 'docker-slave'
            }

            steps {
                echo 'Hello, Maven'
                sh 'mvn -version'
            }

        }
    }
}
