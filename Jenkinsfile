pipeline {
  agent any

  // options {
  //   parallelsAlwaysFailFast()
  // }
  
  stages {
    stage('build') {
      parallel {
        failFast true
        stage('build frontend') {
          steps {
            echo 'build frontend!'
          }
        }

        stage('build backend') {
          steps {
            echo 'build backend!'
          }
        }
      }
    }

    stage('deployment production') {
      steps {
        echo 'deploy !'
      }
    }
  }

}