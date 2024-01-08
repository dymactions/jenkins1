pipeline {
  agent any

  stages {
    stage('build') {
      sh 'echo hello > hello.txt'
      archiveArtifacts(artifacts: '*.txt')
    }
  }

}