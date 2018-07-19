pipeline {
  agent {
    docker {
      image 'ubuntu:latest'
      args '-u root -p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'apt-get install make'
      }
    }
  }
}