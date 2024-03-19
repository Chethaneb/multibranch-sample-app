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
    stage('test456-branch'){
      steps{
        echo "this is for test branch"
        sh "cat README.md"
      }
    }    
  }
} 
