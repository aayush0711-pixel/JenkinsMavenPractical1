
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Validate') {
            steps {
                bat 'mvn validate'
            }
        }

        stage('Compile') {
            steps {
                bat 'mvn compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }

        stage('Verify') {
            steps {
                bat 'mvn verify'
            }
        }

        stage('Install') {
            steps {
                bat 'mvn install'
            }
        }

        stage('Clean') {
            steps {
                bat 'mvn clean'
            }
        }

        stage('Site') {
            steps {
                bat 'mvn site'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Remote Maven repository is not configured; deployment skipped.'
            }
        }
    }
}
