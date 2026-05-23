pipeline {
    agent any
    tools {
        nodejs 'node20' 
    }
    stages {
        stage('build') {
            steps {
                sh 'npm ci'
            }
        }

        stage('run') {
            steps {
                sh 'npm start'
            }
        }

        stage('test') {
            steps {
                sh 'npm test'
            }
        }
    }
}