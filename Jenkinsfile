pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
        }
    agent {
        docker { image 'alpine/helm:2.14.0' }
    }
        stage('Deploy') {
            steps {
                sh 'helm list'
            }
    }
}
}
