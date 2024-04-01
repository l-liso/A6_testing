pipeline {
  agent any
  tools { 
      maven 'maven' 
      jdk 'JDK 21' 
  }
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/l-liso/A6_testing.git', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        sh 'mvn clean' 
        sh 'mvn test' 
        sh 'mvn verify' 
      }
    }
  }
}
