pipeline {
  agent any
  stages {
    stage('Bonjour') {
      steps {
        echo "Hello ${MY_NAME}"
      }      
    }
    stage('La Deuxiemme') {
      steps {
        echo 'Secondary Hello'
      }
    }
    stage('les trois') {
      steps {
        echo 'le trifecta'
      }
    }
    
    stage('Testing') {
        parallel {
          stage('Java 8') {           
            steps {
                sh 'java -version'
              }
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
  environment {
    MY_NAME = 'Diane_1'
  }
  post {
    aborted {
      echo 'Why didn\'t you push my button?'

    }

  }
}
