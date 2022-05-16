pipeline{
    agent any
        stages{
        stage("SSH to remote server"){
            steps{
                sh 'gcloud compute ssh node-server-1 --zone us-central1-a'
                sh 'pwd'
            }
        }
                stage("git clone"){
            steps{
                sh 'rm -rf *'
            sh 'git clone https://github.com/aneksingh00/aneksingh00.git'
                sh 'ls'
                sh 'cd aneksingh00'
                sh 'ls -la'
            }
        }
        stage("npm install"){
            steps{
//                 sh 'sudo apt-get install nodejs -y'
//                 sh 'sudo apt-get install npm -y'
                sh 'npm install'
            }
        }
        stage("npm build"){
            steps{
              
              sh 'node server.js'
            }
        }
    }
}
