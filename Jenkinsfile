pipeline {
  agent {
    dockerfile {
      filename 'gcc:latest'
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