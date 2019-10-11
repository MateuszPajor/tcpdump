pipeline {
  agent any
  stages {
    stage('BUILD') {
      parallel {
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
        stage('') {
          steps {
            sh 'apt add gcc'
          }
        }
      }
    }
  }
}