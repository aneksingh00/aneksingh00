pipeline {
  agent any

    
  stages {
        
    stage('Git') {
      steps {
        git branch: 'main', url: 'https://github.com/aneksingh00/aneksingh00.git'
        sh 'ls -la'
        sh 'cd node-demo'
        sh 'la -la'
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
