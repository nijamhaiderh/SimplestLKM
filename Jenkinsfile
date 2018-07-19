pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'gcc:latest'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''apt-get install linux-headers-4.15.0-23-generic
make'''
      }
    }
  }
}