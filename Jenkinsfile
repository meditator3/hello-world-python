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
        sh 'docker build -t hello-world-python.'
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