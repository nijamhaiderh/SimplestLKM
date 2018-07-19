pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'gcc:latest'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'make --version'
      }
    }
  }
}