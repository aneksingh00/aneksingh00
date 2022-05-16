pipeline {
  agent any

    
  stages {
         stage("SSH to remote server"){
            steps{
                sh 'gcloud compute ssh node-server-1 --zone us-central1-a'
                sh 'pwd'
            }
        }       
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
