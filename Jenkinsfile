pipeline {
agent any
environment {
    JAVA_HOME="C:/jdk-21.0.7"
  }
    tools {
        maven 'Maven_3.6.3'
    }
stages {
stage('Clean stage') {
steps {
dir("product-app-aws") {
bat 'mvn clean'
}
}
}

stage('Compile stage') {
steps {
dir("product-app-aws") {
bat 'mvn compile'
}
}
}

stage('Install stage') {
steps {
dir("product-app-aws") {
bat 'mvn install'
}
}
}

}
}
