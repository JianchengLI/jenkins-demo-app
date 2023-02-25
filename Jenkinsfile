pipeline {
    agent any
    stages {
        stage('Show Gradle Version'){
            steps {
                sh './gradlew --version'
            }
        }
        stage('Build') {
            steps {
                sh './gradlew build -d'
            }
        }
        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }
    }
}
