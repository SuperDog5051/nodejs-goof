pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    def dockerImage = docker.build('nodejs-goof', '--file Dockerfile .')
                }
            }
        }
    }
}
