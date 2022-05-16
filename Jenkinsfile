pipeline {
  agent any

    
  stages {
         stage("SSH to remote server"){
            steps{
                sh 'gcloud compute ssh node-server-1 --zone us-central1-a'
              git branch: 'master', url: 'https://github.com/aneksingh00/aneksingh00.git'
              sh 'ls'
                sh 'pwd'
              sh 'npm install'
              sh 'npm run start'
            }
        }       
  }
}
