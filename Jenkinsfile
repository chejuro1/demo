pipeline {
  agent {
    node {
      label 'maven'
    }

  }
  stages {
    stage('Release') {
      steps {
        sh '''oc project openshift-operators
oc start-build greeting-console  --follow --wait'''
      }
    }

  }
}