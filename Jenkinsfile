pipeline {
  agent none
  stages {
    stage('Saying Hello') {
      steps {
        bat(script: 'echo "Hello World"', returnStatus: true)
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