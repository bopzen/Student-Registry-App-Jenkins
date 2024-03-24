pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from the repository
                git 'https://github.com/bopzen/Student-Registry-App-Jenkins.git'
            }
        }
        
        stage('Installing dependencies') {
            steps {
                // Install Node.js dependencies (replace with your dependency installation command)
                sh 'npm install'
            }
        }
        
        stage('Starting the application') {
            steps {
                // Start the Node.js application in the background
                bat 'start npm start'
            }
        }
        
        stage('Running tests') {
            steps {
                // Run tests (replace with your test command)
                sh 'npm test'
            }
        }
    }
}