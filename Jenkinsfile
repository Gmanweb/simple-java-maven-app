pipeline {

    stages {
        stage('Maven Test') {
            agent {
                docker {
                    label 'scripts'
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
                    label 'scripts'
                    image 'node:7-alpine' 
                }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}
