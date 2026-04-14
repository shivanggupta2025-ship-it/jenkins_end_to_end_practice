pipeline{
    agent any
    stages{
        stage{
            steps{
                checout scm
            }
        }
        stage('Install'){
            steps{
                sh 'npm install'
            }
        }
        stage('Build'){
            steps{
                sh 'echo "Build step..."'
            }
        }
        stage('Deploy'){
            stps{
                sh '''
                mkdir -p /var/www/html/myapp
                cp -r * /var/www/html/myapp
                '''
            }
        }
    }
}