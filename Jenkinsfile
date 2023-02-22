//Jenkins file only to tutorial example
pipeline {
  agent any
    
  stages {
         
    stage('Install dependencies') {
      steps {
        sh 'npm install'
        sh 'npm audit'
      }
    }
    
    stage('Build') {
      steps {
         sh 'npm build'
      }
    } 
    
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}
