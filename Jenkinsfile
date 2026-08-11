pipeline {
    agent {
        label 'linux-agent'
    }

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Agent Test') {
            steps {
                sh 'echo "Pipeline running on Agent"'
                sh 'hostname'
                sh 'whoami'
                sh 'date'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Build completed successfully"'
            }
        }
    }
}
