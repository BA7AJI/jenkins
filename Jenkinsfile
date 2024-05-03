pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker { image 'python:3.9-slim' }
      }
      steps {
        sh 'python --version'
        sh 'echo "print(\'Hello, World!\')" > hello.py'
        sh 'python hello.py'
      }
    }
    stage('Front-end') {
      agent {
        docker { image 'node:16-alpine' }
      }
      steps {
        // Add front-end build steps if needed
      }
    }
  }
}
