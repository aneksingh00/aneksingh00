pipeline{
    agent any
    stages{
        stage("run Docker File"){
            steps{
                sh "docker run -t first:v1 ."
            }
        }
    }
}
