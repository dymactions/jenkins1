pipeline {
  agent any

  parameters {
    string(name: 'NAME', defaultValue: 'M. Jenkins', description: 'Qui est ce ?')
    text(name: 'TEXT', defaultValue: 'un text', description: 'une description')
    booleanParam(name: 'TOGGLE', defaultValue: true, description: 'true ou false')
    choice(name: 'CHOICE', defaultValue: ['un', 'deux', 'trois'], description: 'une liste' )
    password(name: 'PASSWORD', description: 'mot de password')
  }

  stages {
    stage('build') {
      steps {
        echo "NAME : ${ NAME }"
        echo "TEXT : ${ TEXT }"
        echo "TOGGLE : ${ TOGGLE }"
        echo "CHOICE : ${ CHOICE }"
        echo "PASSWORD : ${ PASSWORD }"
      }
    }
  }

}