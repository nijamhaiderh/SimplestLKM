pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'gcc:latest --cap-add=ALL -v /lib/modules:/lib/modules'
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