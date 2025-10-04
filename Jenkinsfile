pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {
        stage('Build') {
            steps {
                echo '🧱 Building the application...'
                sleep 2
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running unit tests...'
                sleep 2
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying to staging environment...'
                sleep 2
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline completed successfully!'
        }
        failure {
            echo '❌ Pipeline failed — please check logs.'
        }
    }
}
