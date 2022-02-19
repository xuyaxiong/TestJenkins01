// Jenkinsfile (Declarative Pipeline)
properties([pipelineTriggers([cron('52 17 * * 1-5')])])

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'scp ./README.md root@123.57.69.247:/var/www/dev.platform.alphesh.com'
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
