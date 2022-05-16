pipeline {
  agent any

    
  stages {
        
    stage('Git') {
      steps {
        git branch: 'master', url: 'https://github.com/aneksingh00/aneksingh00.git'
        sh 'ls -la'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
//          sh '<<Build Command>>'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'npm run start'
      }
    }
  }
}
