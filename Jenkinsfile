pipeline {
    agent any

    environment {
        // Spécifiez le chemin vers Maven
        MAVEN_HOME = 'maven-3.9.6'
        PATH = "$MAVEN_HOME/bin:$PATH"
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Ndaw11/TestDevops.git'
            }
        }

        stage('Build') {
            steps {
                // Utilisez Maven pour construire le projet
                sh 'mvn clean install'
            }
        }

        // Ajoutez d'autres étapes selon vos besoins
    }

    post {
        // Étapes de post-traitement, notifications, etc.
    }
}
