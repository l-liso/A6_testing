pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/l-liso/A6_testing.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}