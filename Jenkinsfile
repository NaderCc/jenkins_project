pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'npm install express'
                sh 'npm install jest'
                sh 'express --version'
                sh 'node -v'
            }
        }
        stage('test') {
            steps {
                sh 'npm test'
            }
        }
    }
}