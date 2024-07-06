pipeline {
  agent none
  stages {
    stage('build') {
      agent { docker { image 'node:20.15.0-alpine3.20' } }
      steps {
        sh 'echo hello world this is '
        // Capture user input for filename (properly indented)
        echo "File '${fileName}' exists: ${fileExists(input message: 'Enter file name', parameters: [string(description: 'user giving input for the filename', name: 'fileName', trim: true)]
)}"
      }
    }
    stage('test') {
      agent { docker { image 'node:20.15.0-alpine3.20' } }
      steps {
        sh 'echo hello world this is '
        // Capture user input for filename (properly indented)
        echo "File '${fileName}' exists: ${fileExists(input message: 'Enter file name', parameters: [string(description: 'user giving input for the filename', name: 'fileName', trim: true)]
)}"
      }
    }

  }
}
