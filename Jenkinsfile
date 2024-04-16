pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from the Git repository
                git 'your-git-repository-url'
            }
        }
        stage('Build') {
            steps {
                // Build the Maven project
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Run tests
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // If needed, deploy the application
                // For example, deploying to a Tomcat server
                // sh 'mvn tomcat7:deploy'
            }
        }
    }
}

