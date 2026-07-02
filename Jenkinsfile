pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code from GitHub...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the Maven project...'
                sh 'mvn clean package'
            }
        }

        stage('Success Message') {
            steps {
                echo '🎉 Build completed successfully!'
            }
        }
    }

    post {
        success {
            echo '✅ GitHub Webhook triggered Jenkins successfully.'
        }

        failure {
            echo '❌ Build failed. Please check the console output.'
        }

        always {
            echo 'Pipeline execution finished.'
        }
    }
}
