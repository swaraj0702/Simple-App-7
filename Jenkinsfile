pipeline {
    agent any

    environment {
        REPO_URL = 'https://github.com/swaraj0702/Simple-App-7.git'
        BRANCH = 'main'
    }

    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning the GitHub repository...'
                git branch: "${BRANCH}", url: "${REPO_URL}"
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add your build commands here (example: compiling code)
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here (example: unit tests)
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add your deployment commands here (example: copying files)
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the error logs.'
        }
    }
}
