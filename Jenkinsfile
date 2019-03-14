#!groovy

pipeline {
    agent any

    stages {
        stage('Maven Test') {
            agent {
                docker {
                    image 'maven:3.3.3'
                }
            }
            steps {
                sh 'mvn test'
            }
        }
    }
}
