pipeline {
  agent {
    docker {
      image 'node:10-alpine'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'node --version'
      }
    }

  }
}