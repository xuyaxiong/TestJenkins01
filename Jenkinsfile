// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sh 'scp ./README.md root@123.57.69.247:/var/www/dev.platform.alphesh.com'
                sh './deploy.sh'
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
