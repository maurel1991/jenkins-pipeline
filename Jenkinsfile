pipeline {
    agent any

    stages {
        stage('CodeScan'){
            steps {
                sh 'trivy fs .  -0 result.html'
            }
        }
        stage('dockerImageBuild'){
            steps {
                sh 'docker -v'
            }
        }
        stage('pushImage'){
            steps{
                sh 'docker ps'
            }
        }
    }
}