pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'javac Main.java'  // Modify based on your project
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'java -jar tests.jar'  // Adjust for your testing framework
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'scp target/app.jar user@server:/deploy/path'  // Modify for deployment
            }
        }
    }
}
