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
    stage('fix-branch'){
      when {
        branch "fix-123"
      } 
      steps{
        sh "cat README.md"
      }
    }    
  }
} 
