pipeline {
  agent any
  stages {
    stage('Bonjour') {
      steps {
        echo 'Hello World'
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
              container('maven8') {
                sh 'mvn -v'
              }
            }
          }
          stage('Java 9') {
            agent { label 'jdk8' }
            steps {
              container('maven9') {
                sh 'mvn -v'
              }
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
}
