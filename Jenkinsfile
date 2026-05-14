pipeline {
    agent any

    stages {
        stage('Dev') {
            steps {
                echo 'I am in dev env'
                echo 'Checking git version'
                sh 'git --version'
                sh 'docker pull nginx'
            }
        }
        stage('staging') {
            steps {
                echo 'I am in staging env'
                echo 'Checking docker version'
                sh 'docker --version'
            }
        }
        stage('Production') {
            steps {
                echo 'I am in production env'
                echo 'Checking docker images'
                sh 'docker images'
            }
        }
    }
}
