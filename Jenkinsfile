pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main',
                    url: 'https://github.com/Aryamnsls/jenkins-pipeline-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage executed'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage executed'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
