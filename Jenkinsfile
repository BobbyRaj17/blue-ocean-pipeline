pipeline {
  // agent { label 'master'}
  // stages {
  //     stage('Test') {
  //         steps {
  //             sh 'docker inspect -f . node:7-alpine'
  //         }
  //     }
  // }
    agent {
        docker { image 'docker:1.12.6' }
    }
    stages {
        stage('Test') {
            steps {
                def customImage = docker.build("my-image:${env.BUILD_ID}")
            }
        }
    }
}
