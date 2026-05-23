pipeline {
    agent any
    tools {
        // لازم السطر ده يكون موجود بالاسم اللي أنت مسميه في الـ Global Tool Configuration
        nodejs 'node20' 
    }
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