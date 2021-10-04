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
      agent {
        dockerfile {
          filename 'dockerfile'
        }

      }
      steps {
        sh 'docker build -t maven .'
      }
    }

  }
}