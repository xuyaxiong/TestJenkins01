// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
//                 bat 'gradlew build'
                sshagent (credentials: ['root']) {
                    sh 'ssh -o StrictHostKeyChecking=no -l cloudbees 123.57.69.247 uname -a'
                }
            }

        }
    }
}
