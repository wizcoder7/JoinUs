pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Checkout code') {   //To checkout based on the configured credentials in the current Jenkins Job

        steps {
            checkout scm
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