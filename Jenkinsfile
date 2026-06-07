pipeline{
    agent any
    environment{
        IMAGE_NAME="python-jenkins-lab"
    }
    stages{
        stage('checkout code'){
            steps{
                git 'https://github.com/Harsh2438/python-jenkins-lab'
            }
        }
        stage('build image'){
            steps{
                bat 'docker build -t python-jenkins-lab .'
            }
        }
        stage('show image'){
            steps{
                bat 'docker images'
            }
        }
    }
}