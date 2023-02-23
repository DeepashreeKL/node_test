//Jenkins file only to tutorial example
pipeline {
  agent any
    
  stages {
         
    stage('INSTALL DEPENDENCIES') {
      steps {
        sh 'npm install'
        sh 'npm audit fix'
      }
    }
    
    stage('BUILD') {
      steps {
         sh 'npm build'
      }
    } 
    
    stage('UNIT TESTING') {
      steps {
         sh 'npm test'
      }
    } 
   
   stage('INTEGRATION TEST'){
      steps {
         sh 'npm verify'
      }
    }

   stage ('CODE ANALYSIS WITH CHECKSTYLE'){
      steps {
         sh 'npm checkstyle:checkstyle'
     }
         post {
            success {
                echo 'Generated Analysis Result'
            }
         }
     }
 
  }
}
