pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "git pull origin master"
                echo 'Build..'
            }
        }
        stage('Test') {
            steps {
                sh "/usr/local/bin/composer update -n"
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