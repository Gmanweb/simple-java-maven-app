pipeline {

    agent {
        label 'scripts'
    }

    stages {
        stage('Docker Version') {
            agent any
            steps {
                sh 'docker --version'
                sh '$HOSTNAME'
                sh 'ls -ltra'
            }
        }
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
        stage('Front-end') {
            agent {
              docker {
                image 'node:7-alpine' 
              }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}
