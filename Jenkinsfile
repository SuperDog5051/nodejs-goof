pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/SuperDog5051/nodejs-goof.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    def dockerImage = docker.build('nodejs-goof', '--file Dockerfile .')
                }
            }
        }
    }
}
