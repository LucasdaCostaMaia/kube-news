pipeline {
  agent any

  stages {

    stage ("Build docker Image") {
      steps {
        script {
          dockerapp = docker.build("lucasdacosta09/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
        }
      }
    }


  }

}