pipeline {
    agent any
    tools {
        maven 'mymaven'
    }
    stages{
        stage('checkout the code'){
            steps{
                git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
        stage('compile the code'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('Run unit Tests'){
            steps{
                sh 'mvn test'
            }
        }
         stage('Build the cde'){
            steps{
                sh 'mvn package'
            }
        }
    }
}

