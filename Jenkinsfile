pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'docker --version'
                sh 'docker images'
                sh 'docker ps'
            }
        }
    }
}
