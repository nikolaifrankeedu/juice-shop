pipeline {
  agent {
    docker {
      image 'nikolaifranke/jenkins:latest'
      args '-p 3000:3000'
    }

  }
  stages {  
    stage('abc') {
      sh 'python script.py'
    }
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
    stage('Start') {
      steps {
        sh 'npm start'
      }
    }
  }
}
