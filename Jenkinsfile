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
        sh 'id'
        sh 'apk add gcc'
        sh './configure'
      }
    }
  }
}