pipeline{
    agent any
    stages{
        stage("run Docker File"){
            steps{
                sh "docker run -t first:v1 ."
            }
        }
    }
        stages{
        stage("Docker images"){
            steps{
                sh "docker images"
            }
        }
    }
}
