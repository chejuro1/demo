pipeline {
  agent {
    node {
      label 'maven'
    }

  }
  stages {
    stage('Release') {
      steps {
        sh '''oc project react-intro2
oc start-build greeting-console  --follow --wait'''
      }
    }

  }
}