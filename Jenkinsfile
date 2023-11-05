pipeline {
    agent any
    stages {
        stage("checkout"){
            steps{
                checkout scm
            }
        }
        
        stage("Test"){
            steps{
                sh 'sudo -S apt install npm'
                sh 'npm test'
            }
        }

        stage("Build"){
            steps{
                sh 'npm run build'
            }
        }
    }
}
