pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''npm config ls && npm install -g npm --registry=https://registry.npm.taobao.org
           '''
      }
    }

  }
}
