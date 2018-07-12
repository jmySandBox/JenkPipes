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
            agent { label 'jdk9' }
            steps {
                sh 'mvn -v'
              }
          }
          stage('Java 9') {
            agent { label 'jdk8' }
            steps {    
                sh 'mvn -v'
            }
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
    TEST_USER = credentials('test-user')
  }
  post {
    aborted {
      echo 'Why didn\'t you push my button?'

    }

  }
}
