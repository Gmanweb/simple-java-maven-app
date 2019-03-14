pipeline {
    agent { label 'php' }
    stages {
        stage("Build") {
            steps {
                echo 'Hello, PHP'
                sh 'php -version'
            }
        }
    }
}