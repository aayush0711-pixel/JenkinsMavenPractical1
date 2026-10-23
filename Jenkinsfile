
node {
    stage('Checkout') {
        checkout scm
    }

    stage('Validate') {
        bat 'mvn validate'
    }

    stage('Compile') {
        bat 'mvn compile'
    }

    stage('Test') {
        bat 'mvn test'
    }

    stage('Package') {
        bat 'mvn package'
    }

    stage('Verify') {
        bat 'mvn verify'
    }

    stage('Install') {
        bat 'mvn install'
    }

    stage('Clean') {
        bat 'mvn clean'
    }

    stage('Site') {
        bat 'mvn site'
    }

    stage('Deploy') {
        echo 'Remote Maven repository is not configured; deployment skipped.'
    }
}
