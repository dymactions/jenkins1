pipeline {
  agent any

  stages {
    stage('build') {
      steps {
        echo 'hello'
      }
    }
   
  }

  post {
    success {
      emailext (to: 'dyma.node@gmail.com', body: '$DEFAULT_CONTENT' , subject: '$DEFAULT_SUBJECT' )   
    }
  }

}