pipeline {
    agent any
    stages {
        stage('Docker Build') {
            steps { sh 'docker build -t hello-app .' }
        }
        stage('Run Container') {
            steps {
                sh 'docker run -d --name hello-app -p 3000:3000 hello-app'
            }
        }
    }
}