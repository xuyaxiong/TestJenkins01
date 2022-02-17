// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent {
        docker { image 'node' }
    }
//     agent any
    stages {
        stage('Build') {
            steps {
//                 sshagent (credentials: ['03d32169-b73b-4370-b225-32d785aef97a']) {
//                     sh 'ssh -o StrictHostKeyChecking=no -l cloudbees 123.57.69.247 uname -a'
//                 }
//                 bat 'java -version'
                sh 'node --version'
            }

        }
    }

    post {
        success {
            echo 'this will run only if successful'
        }
        failure {
            echo 'this will run only if failed'
        }
        always {
            echo 'this will always runs'
        }
    }
}
