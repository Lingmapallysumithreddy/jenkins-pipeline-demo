pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting code from GitHub'
            }
        }

        stage('Build') {
            steps {
                sh 'python3 app.py'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Successful'
            }
        }

    }

    post {
        success {
            echo 'Build Successful'
        }

        failure {
            echo 'Build Failed'
        }
    }
}
