pipeline {
    agent any
    stages {
        stage('compile stage') {
            steps {
                withMaven(maven :'maven3.8.5'){
                sh 'mvn clean compile'
            }
        }
    } 
      stage('Testing stage') {
            steps {
                withMaven(maven :'maven3.8.5'){
                sh 'mvn test'
            }
        }
    } 
      stage('Deployment stage') {
            steps {
                withMaven(maven :'maven3.8.5'){
                sh 'mvn  deploy'
            }
        }
    } 
    }
}
