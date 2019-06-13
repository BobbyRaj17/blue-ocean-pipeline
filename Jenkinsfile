pipeline {
  agent { label 'master'}
  stages {
      stage('Test') {
          steps {
              sh 'docker inspect -f . node:7-alpine'
          }
      }
  }
    // agent {
    //     docker { image 'node:7-alpine' }
    // }
    // stages {
    //     stage('Test') {
    //         steps {
    //             sh 'node --version'
    //         }
    //     }
    // }
}
