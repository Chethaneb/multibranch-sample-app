pipeline {
  agent any
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  stages {
    stage('Build') {
      steps {
        echo "hello"
      }
    }
    stage("README") {
      when {
        branch "fix-*"
      }
      steps {
        sh "cat README.md"
      }
    }
  }
}
  


