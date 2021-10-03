// node('maven') {
//   git 'https://github.com/chejuro1/demo.git' // checks out Dockerfile & Makefile
//   def myEnv = docker.build 'demo:snapshot'
//   myEnv.inside {
//     sh 'make clean install'
//   }
// }

node('maven') {
  git 'https://github.com/chejuro1/demo.git' // checks out Dockerfile and some project sources
  
  withDockerRegistry(credentialsId: 'julescheindjou', toolName: 'docker ', url: 'quay.io/julescheindjou/') {
    // some block
}
  
 docker.withRegistry('https://docker.mycorp.com/', 'docker-login') {
  git '…'
  docker.build('myapp').push('latest')
}
  
}


