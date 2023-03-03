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
            sh 'cd /home/ubuntu/workspace/Job && docker build -t mayank_finalassignment .'
            sh 'docker tag mayank_finalassignment:latest public.ecr.aws/m4q9g4m9/mayank_finalassignment:latest'
            sh 'docker push public.ecr.aws/m4q9g4m9/mayank_finalassignment:latest'
          }
        }        

      }
    }
  }
}
