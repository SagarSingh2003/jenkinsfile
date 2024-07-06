/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:20.15.0-alpine3.20' } }
    stages {
        stage('build') {
            steps {
                sh 'echo hello world this is '
                // Capture user input for filename
                def fileName = input message: 'Enter file name', parameters: [string(description: 'user giving input for the filename', name: 'fileName', trim: true)]
                // Use the captured filename in fileExists check
                echo "File '${fileName}' exists: ${fileExists(fileName)}"
            }
        }
    }
}
