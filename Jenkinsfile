pipeline {
    agent any
 tool 'maven-3.9.6'
    stages {
        stage('Build') {
            steps {
                sh "mvn clean install"
            }
        }
        stage('Test') {
            steps {
                sh "mvn compile"
            }
        }
        // Add stages for Nexus deployment or artifact downloading if needed
    }
}
