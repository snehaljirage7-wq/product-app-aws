
pipeline {
    agent any
 
    tools {
        maven 'Maven3' // Make sure Maven is installed in Jenkins
        jdk 'Java11'   // Make sure JDK is installed in Jenkins
    }
 
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/snehaljirage7-wq/product-app-aws.git'
            }
        }
 
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
 
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
 
        stage('Deploy') {
            steps {
                echo "Deployment stage (Add your AWS/Server commands here)"
            }
        }
    }
 
    post {
        success {
            echo 'Build & Test Successful!'
        }
        failure {
            echo 'Build Failed!'
        }
    }
}
