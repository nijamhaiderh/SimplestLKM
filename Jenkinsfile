pipeline {
  agent {
    docker {
      args '--cap-add=ALL -v /lib/modules:/lib/modules -p 3000:3000'
      image 'gcc:latest'
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