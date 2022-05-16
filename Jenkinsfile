pipeline{
    agent any
        stages{
        stage("SSH to remote server"){
            steps{
                sh 'gcloud compute ssh node-server-1 --zone us-central1-a'
                sh 'pwd'
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
              sh 'cd node-semo'
              sh 'node server.js'
            }
        }
    }
}
