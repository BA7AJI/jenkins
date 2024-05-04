pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker { image 'python:3.8-slim' }
      }
      steps {
        sh 'python --version'
        sh 'echo "Hello, World!"'
      }
    }
    stage('Front-end') {
      agent {
        docker { image 'node:16-alpine' }
      }
      steps {
        sh 'node --version'
      }
    }
  }
}
