pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                sh 'git clone https://github.com/khouloudRb/the-example-app.nodejs.git node'
                sh 'cd node'
                echo 'cloning stage'
            }
        }
        stage('Dependencies installation') {
            steps {
                sh 'npm install'
                echo 'Dependencies installation stage'
            }
        }
        stage('Deploy') {
            steps {
                sh 'npm run start:dev'
                echo 'Deploy stage'
            }
        }
    }
}
