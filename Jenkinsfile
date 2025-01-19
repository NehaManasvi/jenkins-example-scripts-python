pipeline {
  agent {
    docker {
      image 'python:3.12-slim'  // Uses Python 3.8 Docker image
    }
  }
  stages {
    stage('version') {
      steps {
        sh 'python3 --version'  // Checks Python version inside Docker container
      }
    }
    stage('hello') {
      steps {
        sh 'python3 hello.py'  // Executes hello.py script inside Docker container
      }
    }
  }
}
