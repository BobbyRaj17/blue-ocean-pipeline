pipeline {
  agent any
  stages {
    stage('Echo/Test') {
      steps {
        echo 'First crack at this'
      }
    }
  }
  stage('Docker Build') {
            agent {
                docker {
                    reuseNode true    //reuse the workspace on the agent defined at top-level\
                    image 'docker:1.12.6'
                }
            }
            steps {
                sh 'ls'
                sh 'docker version'
            }
        }
}
