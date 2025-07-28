pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/<your-username>/kubernetes-sample-apps.git'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building sample app..."'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying sample app to Kubernetes..."'
            }
        }
    }
}
