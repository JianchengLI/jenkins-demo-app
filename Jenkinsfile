pipeline {
    agent any
    tools {
        gradle '7.6'
    }
    stages {
        stage('Show Gradle Version'){
            steps {
                sh './gradlew --version'
            }
        }
        stage('Build') {
            steps {
                sh './gradlew build -d --no-daemon'
            }
        }
        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }
    }
}
