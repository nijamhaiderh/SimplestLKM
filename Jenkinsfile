pipeline {
  agent {
    node {
      label 'contain'
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
        stage('make') {
          steps {
            sh '''make
dmesg -c
'''
          }
        }
      }
    }
  }
}