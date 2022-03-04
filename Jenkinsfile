// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sh 'scp ./README.md root@123.57.69.247:/var/www/dev.platform.alphesh.com'
                sh './deploy.sh'
            }
            steps {
                sshagent(credentials: ['9da7db0a-1c1c-499f-8bd7-91f78791a55d']) {
                    sh 'ls -la'
                }
            }
        }
    }

    post {
        success {
            echo 'successful'
        }
        failure {
            echo 'failed'
        }
    }
}
