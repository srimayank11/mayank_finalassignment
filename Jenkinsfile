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
            sh 'docker build . -t mayank_finalassignment:latest public.ecr.aws/m4q9g4m9/mayank_finalassignment:latest'             
          }
        }        

      }
    }
  }
}
