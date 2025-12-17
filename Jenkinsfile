pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Pull code from GitHub
                git branch: 'main', credentialsId: 'your-credentials-id', url: 'https://github.com/Samarth-DevTools/devops-repo.git'
            }
        }

        stage('Build') {
            steps {
                // Compile with Maven
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                // Run tests (none here, but placeholder)
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                // Package into JAR
                sh 'mvn package'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy step (placeholder) - e.g., copy JAR to server'
            }
        }
    }
}
