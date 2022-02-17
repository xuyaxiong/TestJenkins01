// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
//                 bat 'gradlew build'
//                 sshagent (credentials: ['root']) {
//                     sh 'ssh -o StrictHostKeyChecking=no -l cloudbees 123.57.69.247 uname -a'
//                 }
                bat 'java -version'
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
