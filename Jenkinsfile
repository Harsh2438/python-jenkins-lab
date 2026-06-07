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
                sh 'docker build -t python-jenkins-lab .'
            }
        }
        stage('show image'){
            steps{
                sh 'docker images'
            }
        }
    }
}