pipeline {
  agent {
    docker {
      image 'gcc:latest'
      args '-it --cap-add=ALL -v /lib/modules:/lib/modules -v /usr/src:/usr/src'
    }

  }
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''
ls -al /lib/modules/4.15.0-23-generic/'''
          }
        }
        stage('ls user src') {
          steps {
            sh 'ls -al /usr/src/'
          }
        }
      }
    }
  }
}