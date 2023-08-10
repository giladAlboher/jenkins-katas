pipeline {
  agent any
  tools{
    gradle 'gradle 8.3'
    dockerTool 'docker'
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
            sh 'cd ci && ./build-app.sh'
          }
        }

      }
    }

  }
}
