#!groovy

pipeline {

    agent { 
        label 'agent_temp'
    }

    stages {

        stage("list") {
            steps {
                echo 'Hello, Docker'
                sh 'ls -ltra'
                sh 'echo $HOSTNAME'
                sh 'mvn -version'
            }
        }
    }
}