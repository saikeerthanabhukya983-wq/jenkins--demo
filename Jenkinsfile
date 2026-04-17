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
                echo 'No tests configured'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'

                // Copy file to a simple location (optional)
                bat 'dir'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Opening calculator...'
                bat 'start calculator.html'
            }
        }
    }
}
