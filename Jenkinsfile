pipeline {
    agent any
    stages {
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
