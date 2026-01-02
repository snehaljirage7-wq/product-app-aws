pipeline {
agent any
environment {
    JAVA_HOME="C:\Program Files\Java\jdk-21.0.9"
  }
stages {
stage('Clean stage') {
steps {
dir("product-app-aws") {
bat 'C:/maven/apache-maven-3.9.9/bin/mvn clean'
}
}
}

stage('Compile stage') {
steps {
dir("product-app-aws") {
bat 'C:/maven/apache-maven-3.9.9/bin/mvn compile'
}
}
}

stage('Install stage') {
steps {
dir("product-app-aws") {
bat 'C:/maven/apache-maven-3.9.9/mvn install'
}
}
}

}
}
