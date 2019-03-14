#!groovy

pipeline {

    agent {
        label 'mvn-slave'
    }

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
