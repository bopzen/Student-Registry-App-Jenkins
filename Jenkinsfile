pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from the repository
                git 'https://github.com/bopzen/Student-Registry-App-Jenkins.git'
            }
        }
        
        stage('Setting up Node.js') {
            steps {
                // Install Node.js (replace with your Node.js setup steps if needed)
                sh 'curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -'
                sh 'sudo apt-get install -y nodejs'
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
                // Start the Node.js application (replace with your start command)
                sh 'npm start &'
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