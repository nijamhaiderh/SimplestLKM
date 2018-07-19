pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image '60dc8024350f'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'whoami'
      }
    }
  }
}