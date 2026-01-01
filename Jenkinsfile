pipeline {
    agent any

    environment {
        JAVA_HOME = "C:/jdk-21.0.7"
        PATH = "${JAVA_HOME}/bin;${env.PATH}"
    }

    tools {
        maven 'Maven_3.6.3'
    }

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Clean') {
            steps {
                bat 'mvn clean'
            }
        }

        stage('Compile') {
            steps {
                bat 'mvn compile'
            }
        }

        stage('Install') {
            steps {
                bat 'mvn install'
            }
        }
    }
}
