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
        sh '''/bin/bash,
	su root,
	apt-get update,
	apt-get install make'''
      }
    }
  }
}
