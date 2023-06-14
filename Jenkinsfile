pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'git@github.com:meditator3/hello-world-python.git', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        sleep 4
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