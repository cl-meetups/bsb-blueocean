pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo 'Hello World'
      }
    }
    stage('Paralelo') {
      steps {
        parallel(
          "Paralelo": {
            sh 'date'
            
          },
          "Sleep": {
            sleep 10
            
          }
        )
      }
    }
    stage('Final') {
      steps {
        echo 'Finalizando'
      }
    }
  }
}