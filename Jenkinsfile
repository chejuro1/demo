pipeline {
  agent {
    node {
      label 'maven'
    }

  }
  stages {
    stage('Release') {
      steps {
        sh '''ls 
oc project react-intro2
oc start-build greeting-console  --follow --wait'''
      }
    }

    stage('Docker_lint') {
      steps {
        sh '''npm install -g dockerlint
dockerlint Dockerfile'''
      }
    }

  }
}