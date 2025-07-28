pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Abhinay2510/kubernetes-sample-apps.git'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building sample app..."'
            }
        }
        stage('Deploy') {
    steps {
        sh '''
        kubectl apply -f deployment.yaml
        '''
    }
}

    }
}
