pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Fetching code from GitHub...'
            }
        }

        stage('Build') {
            steps {
                echo 'No build needed for HTML project'
            }
        }

        stage('Test') {
            steps {
                echo 'Checking if index.html exists...'
                bat 'if exist index.html (echo File exists) else (exit 1)'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '*.html', fingerprint: true
            }
        }
    }
}
