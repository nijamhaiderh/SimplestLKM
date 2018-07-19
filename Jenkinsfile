pipeline {
  agent {
    docker {
      image 'gcc:latest'
      args '-u root --cap-add=ALL -v /lib/modules:/lib/modules -v /usr/src:/usr/src'
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
insmod hello.ko
dmesg
rmmod hello.ko
dmesg
'''
          }
        }
      }
    }
  }
}