//Jenkins file only to tutorial example
pipeline {
  agent any
    
  stages {
         
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
    
    stage('Build') {
      steps {
         sh 'npm run build'
      }
    } 
    
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}
