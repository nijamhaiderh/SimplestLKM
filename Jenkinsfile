pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'ubuntu:latest'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''/bin/bash
apt-get update\\n apt-get install make\\n make'''
      }
    }
  }
}