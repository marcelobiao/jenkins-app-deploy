pipeline {
    agent { node {label 'master'}}
    stages {
        stage('Build') {
            steps {
                sh 'composer install'
            }
        }
        stage('Test') {
            steps {
                sh 'vendor/bin/phpunit'
            }
        }
    }
}