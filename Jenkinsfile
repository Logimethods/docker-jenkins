pipeline {
    agent none
    stages {
        stage('mvn') {
            agent { docker 'maven:3.3.3' }
            steps {
                sh 'mvn --version'
            }
        }
        stage('docker') {
            agent any
            try {
                sh 'docker --version'
            }
            catch (exc) {
                echo "$exc"
            }
        }
    }
}
