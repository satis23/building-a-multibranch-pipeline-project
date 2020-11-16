pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
        }
        stage('Deploy') {
    agent {
        docker { image 'alpine/helm:2.14.0' }
    }
            steps {
                container('docker'){
                sh 'helm list'
                }
            }
    }
}
}
