pipeline {
agent any
environment {
    JAVA_HOME="C:/jdk-21.0.7"
  }
stages {
stage('Clean stage') {
steps {
dir("product-app-aws") {
bat '"C:/Users/SJ68573/apache-maven-3.6.3-bin 3/apache-maven-3.6.3/bin/mvn" clean'
}
}
}

stage('Compile stage') {
steps {
dir("product-app-aws") {
bat '"C:/Users/SJ68573/apache-maven-3.6.3-bin 3/apache-maven-3.6.3/bin/mvn" compile'
}
}
}

stage('Install stage') {
steps {
dir("product-app-aws") {
bat '"C:/Users/SJ68573/apache-maven-3.6.3-bin 3/apache-maven-3.6.3/bin/mvn" install'
}
}
}

}
}
