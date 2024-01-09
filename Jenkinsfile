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
      emailext (to: 'dyma.node@gmail.com', body: 'test body' , subject: 'test subject jenkins' )   
    }
  }

}