pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package -DskipTests' // Baut das Projekt mit Maven, überspringt Tests
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test' // Führt Tests aus
            }
        }
    }
}