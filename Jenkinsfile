pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git pull
                echo 'Build..'
            }
        }
        stage('Test') {
            steps {
                composer install
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