pipeline {
  agent any
  stages {
    stage('BUILD') {
      parallel {
        stage('BUILD') {
          steps {
            sh 'echo \'hello\''
          }
        }
        stage('') {
          steps {
            sh 'pwdls -la'
          }
        }
      }
    }
  }
}