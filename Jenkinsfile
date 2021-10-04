// node('maven') {
//   git 'https://github.com/chejuro1/demo.git' // checks out Dockerfile & Makefile
//   def myEnv = docker.build 'demo:snapshot'
//   myEnv.inside {
//     sh 'make clean install'
//   }
// }

// node('maven') {
//   git 'https://github.com/chejuro1/demo.git' // checks out Dockerfile and some project sources
  
//   withDockerRegistry(credentialsId: 'julescheindjou', toolName: 'docker ', url: 'quay.io') {

//   docker.build('myapp').push('latest')
// }
  
 
  
// }

// node('maven' {
//     checkout scm

//     docker.withRegistry('https:/quay.io', 'julescheindjou') {

//         def customImage = docker.build("my-image:${env.BUILD_ID}")

//         /* Push the container to the custom Registry */
//         customImage.push()
//     }
// }

pipeline {
   agent any
   stages {
      stage('Hello') { 
         steps {
            echo 'Hello World!'
         }
      }
   }
}


