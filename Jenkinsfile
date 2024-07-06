pipeline {
  agent none
  stages {
    stage('build') {
      agent { docker { image 'node:20.15.0-alpine3.20' } }
      steps {
        sh 'echo hello world this is '
        // Capture user input for filename (properly indented)
        echo  ' Hello world !!!!! node:20 '
      }
    }
    stage('test') {
      agent { docker { image 'node:20.15.0-alpine3.20' } }
      steps {
        sh 'echo hello world this is '
        // Capture user input for filename (properly indented)
        echo "Hello World 2 "
      }
    }

  }
}
