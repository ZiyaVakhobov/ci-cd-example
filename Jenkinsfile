pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "git pull"
                echo 'Build..'
            }
        }
        stage('Test') {
            steps {
                sh "composer install"
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}