pipeline {
  agent {
    docker {
      image 'node:10-alpine'
    }

  }
  stages {
    stage('Build') {
      agent {
        docker {
          image 'node:10-alpine'
        }

      }
      steps {
        sh 'node --version'
      }
    }

  }
}