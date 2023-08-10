pipeline {
  agent any
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
            sh 'sleep infinity'
            sh 'cd ci && ./build-app.sh'
          }
        }

      }
    }

  }
  tools {
    gradle 'gradle 8.3'
    dockerTool 'docker'
  }
}
