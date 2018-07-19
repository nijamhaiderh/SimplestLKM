pipeline {
  agent {
    docker {
      image 'gcc:latest'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''
make'''
      }
    }
  }
}