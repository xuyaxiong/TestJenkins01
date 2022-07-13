pipeline {
  agent {
    docker {
      image 'node:10-alpine'
      args '-u root'
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