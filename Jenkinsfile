pipeline {  
  agent any  
  stages {
    stage('Git Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Build Docker Image') {
      parallel {
        stage('Build Docker Image') {
          steps {
            sh 'echo mayank'
            sh 'cd /home/ubuntu/workspace/Job && sudo docker build .
          }
        }        

      }
    }
  }
}
