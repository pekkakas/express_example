pipeline {
  agent {
    docker {
      image 'node:8-alpine'
      args 'Args: -p 3000:3000'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        sh 'npm test'
      }
    }

  }
  environment {
    Start = ''
  }
}