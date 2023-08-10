pipeline {
  agent any
  stages {
    stage('hello') {
      parallel {
        stage('hello') {
          steps {
            sh 'echo "hello world"'
          }
        }

        stage('buildApp') {
          steps {
            sh '''echo "buildApp

'''
          }
        }

      }
    }

  }
}