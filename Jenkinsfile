pipeline {

    // agent {
    //     label 'scripts'
    // }

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
