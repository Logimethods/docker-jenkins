pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('mvn') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('docker') {
            try {
                sh 'docker --version'
            }
        }
    }
}
