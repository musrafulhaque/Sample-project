pipeline {
    agent any
    stages {
        stage ('Clone git repo') {
            steps {
                git 'https://github.com/musrafulhaque/Sample-project.git'
            }
        }
        stage('Starting the website') {
            steps {
                script {
                    sh 'docker build -t mushuru-hello .'
                    sh 'docker run mushuru-hello'
                }
            }
        }
    }
}