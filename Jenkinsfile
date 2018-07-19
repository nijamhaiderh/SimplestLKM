pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'ubuntu:latest festive_wozniak'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'whoami'
      }
    }
  }
}