pipeline {
  agent any
  stages {
    stage('BUILD') {
      agent {
        docker {
          image 'alpine'
        }

      }
      steps {
        sh './configure'
      }
    }
  }
}