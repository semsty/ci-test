pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                checkout scm
            }
        }
        stage('Test') {
            steps {
                sh './ci-test'
            }
        }
    }
    post {
        always {
            echo 'Done'
        }
    }
}