scripts
pipeline {
    agent any

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

    }
}
