pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/meditator3/hello-world-python.git', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -t arielguez/hello-world-python:$BUILD_NUMBER .'
      }
    }

    stage('Test') {
      steps {
        sh 'docker run -itd hello-world-python -p 8080:8080 arielguez/hello-world-python:$BUILD_NUMBER '
      }
    }

    stage('Push') {
      steps {
        sleep 1
      }
    }

  }
}