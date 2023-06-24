pipeline {
    agent none
    stages {
        stage('Back-end') {
            agent {
                docker { image 'maven:3.9.0-eclipse-temurin-11' }
            }
            steps {
                sh 'mvn --version'
            }
        }
        stage('Front-end') {
            agent {
                docker { image 'node:18.16.0-alpine' }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}
