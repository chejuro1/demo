pipeline {
  agent {
    node {
      label 'maven'
    }

  }
  stages {
    stage('Hello') {
      steps {
        echo 'Hello World!'
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -t maven .'
      }
    }

  }
}