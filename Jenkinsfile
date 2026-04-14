pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install') {
            steps {
                bat 'npm install'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Build step...'
            }
        }

        stage('Deploy') {
    steps {
        cleanWs()
        bat 'echo Clean deploy'
    }
}
    }
}