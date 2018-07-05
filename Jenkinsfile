pipeline {
  agent any
  stages {
    stage('Saying Hello') {
      steps {
        bat(script: 'echo Hello World', returnStatus: true)
      }
    }
    stage('La Deuxiemme Salut') {
      steps {
        bat 'echo Secondary Hello'
      }
    }
    stage('les trois') {
      steps {
        bat 'echo le trifecta'
      }
    }
    stage('le fin') {
      steps {
        echo 'I am Your Master - Thou Shalt Obey Me'
      }
    }
    stage('qui ma dire') {
      steps {
        echo 'You changed me'
      }
    }
  }
}