node('maven') {
  git 'https://github.com/chejuro1/demo.git' // checks out Dockerfile & Makefile
  def myEnv = docker.build 'my-environment:snapshot'
  myEnv.inside {
    sh 'make test'
  }
}
