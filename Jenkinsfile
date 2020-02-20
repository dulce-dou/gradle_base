pipeline {
    agent {label 'swarm'}
    stages {
        stage('Build') {
            steps {
                sh './gradlew build'
            }
        }
        stage('Test') {
            steps {
                sh './gradlew clean test --no-daemon'
            }
        }
    }
}
