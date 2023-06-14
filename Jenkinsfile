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
        sleep 4
      }
    }

    stage('Push') {
      steps {
        sleep 1
      }
    }

  }
}