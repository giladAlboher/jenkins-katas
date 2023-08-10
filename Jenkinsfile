pipeline {
  agent {
    docker {
      image 'gradle:6-jdk11'
    }

  }
  stages {
    stage('Parallel execution') {
      parallel {
        stage('hello') {
          steps {
            sh 'echo "hello world"'
          }
        }

        stage('buildApp') {
          steps {
            sh 'echo "lalalalala"'
          }
        }

      }
    }

  }
}