// Jenkinsfile (Declarative Pipeline)
pipeline {
//     agent {
//         docker { image 'node' }
//     }
    agent any
    stages {
        stage('Build') {
            steps {
                sshagent (credentials: ['98ebaf21-bf54-4e95-80a2-c53570c26365']) {
//                     sh 'ssh -o StrictHostKeyChecking=no -l root 123.57.69.247 uname -a'
                    sh 'scp ./README.md jenkins@123.57.69.247:/var/www/dev.platform.alphesh.com'
                }
                sh 'java -version'
//                 sh 'node --version'
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
