pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/l-liso/A6_testing.git', branch: 'master')
      }
    }

    stage('run') {
      agent any
      steps {
        sh 'mvn verify'
      }
    }

  }
  environment {
    maven = 'maven'
    jdk = 'JDK 21'
  }
}