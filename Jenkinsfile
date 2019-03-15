#!groovy

pipeline {

    agent { 
        label 'agent_maven'
    }

    stages {

        stage("list") {
            steps {
                echo 'Hello, Docker'
                sh 'ls -ltra'
                sh 'echo $HOSTNAME'
                sh 'mvn -version'
                sh 'sleep 1m'
            }
        }
    }
}