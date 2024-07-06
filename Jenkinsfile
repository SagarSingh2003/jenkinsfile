/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:20.15.0-alpine3.20' } }
    stages {
        stage('build') {
            steps {
                sh 'echo hello world this is '
               fileExists '/output.txt'
            }
        }
    }
}
