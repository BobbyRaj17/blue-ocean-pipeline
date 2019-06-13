pipeline {
  agent any
  stages {
      stage('Test') {
          steps {
              sh 'whoami'
          }
      }
  }
    agent {
        docker { image 'node:7-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
