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
        docker {
          image 'docker:19.03.12'
          args '''--docker-volumes "/certs/client"
 --docker-privileged'''
        }

      }
      steps {
        sh 'docker build -t maven .'
      }
    }

  }
}