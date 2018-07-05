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
        stage('en Francaise') {
          steps {
            echo 'I am Your Master - Thou Shalt Obey Me'
          }
        }
      }
    }
  }
}