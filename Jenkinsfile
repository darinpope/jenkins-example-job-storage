pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        sh 'echo Hello > hello.txt'
      }
    }
  }
  post {
    success {
      archiveArtifacts artifacts: 'hello.txt', followSymlinks: false
    }
  }
}
