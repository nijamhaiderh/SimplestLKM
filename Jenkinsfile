pipeline {
  agent {
    dockerfile {
      filename 'gcc:latest -v /lib/modules:/lib/modules'
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