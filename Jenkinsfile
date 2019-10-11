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
        stage('gcc') {
          steps {
            sh 'apt add gcc'
          }
        }
        stage('id') {
          steps {
            sh 'id; whoaim'
          }
        }
      }
    }
  }
}