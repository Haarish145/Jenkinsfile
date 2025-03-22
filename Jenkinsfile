pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/your-repo.git'  // Replace with your repo URL
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'javac MyApp.java'  // Compile Java files
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'java -jar test-runner.jar'  // Run unit tests
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'scp MyApp.jar user@server:/deploy/path'  // Deploy via SCP
            }
        }
    }
}
