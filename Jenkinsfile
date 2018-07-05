pipeline {
  agent any
  stages {
    stage('Saying Hello') {
      parallel {
        stage('Saying Hello') {
          steps {
            bat(script: 'echo Hello World', returnStatus: true)
          }
        }
        stage('Say Bye') {
          steps {
            bat 'echo GoodBye Friend'
          }
        }
      }
    }
  }
  environment {
    stages = ''
    stage = 'Hello World'
    steps = ''
    echo = 'Saying Hello'
  }
}