pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('checkout') {
      steps {
        git(url: 'git@github.com:meditator3/hello-world-python.git', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        sh 'docker build .'
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