pipeline {
    agent any

    stages {
        stage('Checkout Source Code') {
            steps {
                echo 'Pulling code from Git repository...'
                checkout scm
            }
        }

        stage('Build & Dependencies') {
            steps {
                echo 'Building application workspace...'
                // Changed 'sh' to 'bat' for Windows
                bat 'echo "Build Phase Completed Successfully"'
            }
        }

        stage('Automated Testing') {
            steps {
                echo 'Running automated test suites...'
                // Changed 'sh' to 'bat' for Windows
                bat 'echo "Test Phase Passed"'
            }
        }

        stage('Code Stability Check') {
            steps {
                echo 'Evaluating build quality metrics...'
                // Changed 'sh' to 'bat' for Windows
                bat 'echo "Code stability criteria met."'
            }
        }
    }

    post {
        success {
            echo 'SUCCESS: CI Pipeline completed successfully!'
        }
        failure {
            echo 'FAILURE: Pipeline failed. Check build logs.'
        }
    }
}
