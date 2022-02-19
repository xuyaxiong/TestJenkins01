// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {

                sh 'scp ./README.md root@123.57.69.247:/var/www/dev.platform.alphesh.com'

                sh 'ssh -o StrictHostKeyChecking=no -l root 123.57.69.247 uname -a'
                sh 'ls -la'
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
