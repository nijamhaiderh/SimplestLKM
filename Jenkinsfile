pipeline {
  agent {
    docker {
      image 'gcc:latest'
      args '--cap-add=ALL -v /lib/modules:/lib/modules'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''
ls -al /lib/'''
      }
    }
  }
}