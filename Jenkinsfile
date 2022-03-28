pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'echo "Hello World"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "success"'
            }
        }
    }
}
