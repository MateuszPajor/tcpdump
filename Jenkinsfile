pipeline {
  agent any
  stages {
    stage('BUILD') {
      agent {
        docker {
          image 'alpine'
          args '-u 0'
        }

      }
      steps {
        sh 'id'
        sh 'apk add gcc;'
        sh './configure'
      }
    }
  }
}