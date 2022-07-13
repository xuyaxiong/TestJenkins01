pipeline {
  agent none
  stages {
    stage('Build') {
      agent {
        docker {
          args '-u root'
          image 'node:10-alpine'
        }

      }
      steps {
        sh 'node --version'
      }
    }

  }
}