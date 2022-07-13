pipeline {
  agent none
  stages {
    stage('Build') {
      agent {
        docker {
          args '-u root'
          image 'node:latest'
        }

      }
      steps {
        sh 'node --version'
      }
    }

  }
}