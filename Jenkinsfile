pipeline {
  agent {
    docker {
      image 'node:ubuntu'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'make'
      }
    }
  }
}
