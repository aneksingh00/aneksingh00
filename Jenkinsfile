pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git branch: 'main', url: 'https://github.com/aneksingh00/aneksingh00.git'
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
        sh 'node start'
      }
    }
  }
}
