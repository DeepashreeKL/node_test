//Jenkins file only to tutorial example
pipeline {
  agent any
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/DeepashreeKL/node_test.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}
